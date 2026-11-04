# 笔记本电脑 AI 导购 Agent

通过产品设计、Agent Harness 设计、AI Coding 和评估验证，逐步实现可运行的 MVP。

> 当前状态：项目目录与文档模板已初始化，尚未实现可运行 Demo。文档中的待办和建议参数需要在开发前确认。

## 项目目标

在有限商品目录和用途适配依据上，让单 Agent 根据当前信息选择澄清、检索、核验或推荐行动。程序强制校验硬条件与证据，避免无依据推荐。

## 目录导航

| 路径 | 用途 |
| --- | --- |
| [docs/01_Project_Brief.md](docs/01_Project_Brief.md) | 定位、用户问题与 MVP 边界 |
| [docs/02_PRD.md](docs/02_PRD.md) | 功能需求与用户交互 |
| [docs/03_Agent_Harness.md](docs/03_Agent_Harness.md) | 状态、行动、循环与约束 |
| [docs/04_Data_Tools.md](docs/04_Data_Tools.md) | 数据与工具输入输出 |
| [docs/05_Evaluation.md](docs/05_Evaluation.md) | 测试场景与验收标准 |
| [docs/06_Development_Plan.md](docs/06_Development_Plan.md) | AI Coding 分阶段任务 |
| src/app/ | 页面与 API |
| src/components/ | 聊天、条件、商品卡片等组件 |
| src/agent/ | Prompt、执行循环、状态与工具注册 |
| src/tools/ | 商品检索、详情读取与证据检索 |
| src/rules/ | 硬条件、用途适配和输出校验 |
| src/lib/ | 数据访问和通用能力 |
| data/ | 商品目录与适配规则 |
| tests/ | 规则测试与 Agent 场景测试 |
| evidence/ | 执行轨迹、开发记录与演示证据 |

## 开发起点

1. 完善项目定位、Harness、数据工具与验收文档。
2. 按开发计划搭建 UI，再实现确定性规则，最后接入真实模型。
3. 每个阶段记录修改、验证结果及未解决问题。

拟采用 Next.js + TypeScript；具体依赖和 Agent 框架版本在实现阶段验证并锁定。目前没有 package.json 或启动命令，不能执行 npm run dev。

## 配置与安全

未来接入模型时参考 [.env.example](.env.example)，将真实密钥保存在本地 .env.local。不要将密钥放入客户端代码、Git 或演示记录。

## 演示与结果

- Demo 地址：待开发后补充。
- 测试结果：待实际执行后记录。
- AI Coding 记录：见 evidence/ai-coding/。
