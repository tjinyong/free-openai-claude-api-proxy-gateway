---
layout: default
title: NewAPI vs Sub2API：YesAPI 后台迁移与程序对比
description: 对比 NewAPI 和 Sub2API 这两个 AI API 网关程序的用户、API Key、额度、渠道和后台迁移差异，说明如何在保留 YesAPI 品牌的情况下更换后台。
permalink: /docs/reviews/new-api-vs-sub2api-migration/
---

# NewAPI vs Sub2API：YesAPI 后台迁移与程序对比

先澄清三个概念：

- **YesAPI** 是对外的品牌、网站和 API 服务名称；
- **Sub2API** 是当前使用的后台程序；
- **NewAPI** 是另一个开源的 AI API 网关程序。

NewAPI 和 Sub2API 都不是模型服务商，也不是和 OpenRouter、YesAPI 同一层级的产品。它们负责用户管理、API Key、渠道转发、模型路由、额度统计和后台运营；真正提供模型能力的是配置在网关后面的上游渠道。

## 更换后台后，YesAPI 品牌可以保留吗？

可以。更换 NewAPI 不要求更换 YesAPI 品牌，也不要求更换对外域名。需要保留的内容包括：

- YesAPI 官网和控制台域名；
- 对外 API 域名；
- README、文档和推广链接；
- 用户看到的产品名称和 Logo；
- 对外的价格、余额和服务规则。

NewAPI 只作为 YesAPI 的底层网关程序使用。NewAPI 自带的前端界面、Logo 和默认文案则需要按 YesAPI 的品牌进行定制，或者继续使用现有前端并增加接口适配层。

## NewAPI 和 Sub2API 的主要差异

| 维度 | Sub2API | NewAPI |
| :--- | :--- | :--- |
| 定位 | API 分发与运营平台 | AI API 聚合与网关平台 |
| 用户系统 | 有自己的用户、余额、订阅和支付模型 | 有自己的用户、Token、额度和权限模型 |
| API Key | 使用 Sub2API 自己的存储和鉴权逻辑 | 使用 NewAPI 自己的 Token 和鉴权逻辑 |
| 渠道配置 | Sub2API 渠道、账号和模型配置 | NewAPI 渠道、分组和模型路由配置 |
| 计费字段 | 余额、订阅、用量和支付订单 | Quota、Token 用量、倍率和计费配置 |
| 数据库 | 当前 Sub2API 的独立数据模型 | NewAPI 的独立数据模型 |
| 外部客户端 | 主要通过 OpenAI-compatible API 调用 | 支持 OpenAI-compatible 以及其他兼容格式 |

两者都能提供类似的 `/v1` API 入口，但“接口格式相似”不代表“后台数据库兼容”。

## 用户能否直接迁移？

不能直接复制数据库后启动。可迁移性需要逐项处理：

| 数据 | 迁移建议 |
| :--- | :--- |
| 用户名、邮箱、状态 | 编写字段映射后迁移 |
| 用户余额 | 可以迁移，但必须核对额度单位和精度 |
| 订阅与用户分组 | 需要转换 NewAPI 对应字段 |
| API Key | 建议重新生成，不能默认沿用旧 Key |
| 登录 Session | 不迁移，要求用户重新登录 |
| 渠道和上游密钥 | 重新配置或按加密格式转换 |
| 使用记录 | 可归档，不能假定统计字段完全一致 |
| 支付订单 | 单独保留原系统记录，必要时做对账迁移 |

因此更准确的说法是：**用户可以迁移，不能做无验证的数据库直拷贝。**

## 外部 API 用户会不会受影响？

如果继续使用原来的 API 域名，并让新后台保持相同的请求入口，客户端配置可以尽量不变：

```text
Base URL: 原来的 YesAPI API 地址
API Key:  切换后重新签发的 Key
Model:    新后台中实际配置的模型名
```

但旧 API Key 是否继续有效，取决于是否实现了旧 Key 到 NewAPI Token 的兼容映射。最稳妥的切换方式是提前通知用户重新创建 Key，并保留一段时间的旧系统只读或兼容验证能力。

## 推荐迁移顺序

1. 保留 YesAPI 域名和品牌不变。
2. 单独部署 NewAPI 测试实例。
3. 导出 Sub2API 用户、余额、分组和渠道配置。
4. 编写并运行一次性字段转换脚本。
5. 抽样核对用户数量、余额总额、分组和模型路由。
6. 让内部用户测试登录、充值、API 调用和余额扣除。
7. 正式切换前冻结充值和关键配置变更。
8. 切换反向代理或域名指向 NewAPI。
9. 观察错误率、扣费记录和用户登录情况。

不要直接在生产数据库上运行未经验证的 `INSERT` 或 `UPDATE`。先备份原库，在隔离数据库完成导入和对账，再执行正式切换。

## 结论

NewAPI 和 Sub2API 是后台程序之间的替换关系，不是模型供应商之间的选择。YesAPI 可以继续作为品牌和服务名称保留；需要改的是底层部署、数据库迁移、用户鉴权、API Key、渠道配置和计费适配。

相关项目：[NewAPI](https://github.com/QuantumNous/new-api)；当前业务入口：[YesAPI 控制台](https://yesapi.online/?utm_source=github&utm_medium=migration)。
