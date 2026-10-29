#  E'Angelo here 👋


## 🚀 旗舰项目

**[tapedeck](https://github.com/EAnge1o/tapedeck)** — LLM Agent 飞行记录仪 ⏺
*Record once (REC), replay forever offline for free (PLAY), diff what drifted. Zero dependencies.*

把 Agent 的一次完整运行（模型调用、工具调用、usage）录成带版本号的 JSONL trace；改完代码离线逐字节重放，零 API 成本；两个 run 一条命令 diff，直接定位第一个漂移的步骤。纯标准库零依赖，diff 退出码直连 CI 做回归测试。`tape.watch(client)` 还能直接拦截 OpenAI / Anthropic / DeepSeek SDK 的调用（含流式），不改业务代码就有录制与重放；自带 pytest fixture。`pip install tapedeck-llm`。

姊妹工具 📼 **[mocktape](https://github.com/EAnge1o/mocktape)** — 同一个"磁带"隐喻用在 HTTP 层：一份配置文件生成带状态的 CRUD 接口，真实 API 录制成磁带离线回放，未命中请求给出「最近匹配」诊断，支持场景切换、故障注入与实时流量面板。mocktape 管 HTTP 流量，tapedeck 管 agent 决策，常常一起出现在同一个测试套件里。

## 🏆 比赛 · Kaggle · 黑客松

**Kaggle**
- **[Predicting-Airline-Satisfaction](https://github.com/EAnge1o/Predicting-Airline-Satisfaction)** — Kaggle Playground S6E10：固定折验证 + 航线特征 + 嵌套 OOF 堆叠，公开榜 AUC `0.96213`（当时 122 / 3142）
- **[Kaggle-Google-The-Gemma-4-Developer-Agent](https://github.com/EAnge1o/Kaggle-Google-The-Gemma-4-Developer-Agent)** — 基于 Gemma 4 的开发者 Agent 方案 🚧 *进行中*

**比赛**
- **[mcd-repeat-smarter](https://github.com/EAnge1o/mcd-repeat-smarter)** — 麦麦老样子：基于麦当劳官方 MCP 的个性化点餐助手 ⭐10 · 麦当劳程序员创意开发大赛 🚧 *进行中*
- **[midnight-oracle](https://github.com/EAnge1o/midnight-oracle)** — 镜映心：离线「塔罗 + 答案之书」小工具，全程 0 网络请求 · [在线体验](https://eange1o.github.io/midnight-oracle/) · 小红书小工具创意大赛 🚧 *进行中*

**黑客松**
- **[ARC-Prize-2026-ARC-AGI-3](https://github.com/EAnge1o/ARC-Prize-2026-ARC-AGI-3)** — ARC Prize 2026（ARC-AGI-3）求解方案 🚧 *进行中*
- **TruLens · 欧莱雅黑客松** — 面向美妆种草内容的多模态真实性核验 Agent：四维可信度分析 + 多 Agent 架构（源码在私人仓库）
- **[octos-arc](https://github.com/EAnge1o/octos-arc)** — ARC-Bench 黑客松：自主软件工程 Agent，需求文档 + 参考图 → 可运行全栈 Web 应用

## ⚙️ Nimbus 系列

- **[nimbus-infer-rs](https://github.com/EAnge1o/nimbus-infer-rs)** — 纯 std 的 Rust LLM 推理引擎：手写 AVX2/FMA 内核，int4 解码吞吐 +85%
- **[nimbus-infer](https://github.com/EAnge1o/nimbus-infer)** — 纯 NumPy 的 LLM 推理引擎：BPE / KV Cache / int8·int4 量化
- **[nimbus-vm](https://github.com/EAnge1o/nimbus-vm)** — 字节码虚拟机，自带 mark-sweep GC
- **[nimbus-git](https://github.com/EAnge1o/nimbus-git)** — Git 对象模型：objects / index / refs
- **[nimbus-db](https://github.com/EAnge1o/nimbus-db)** — SQL 数据库引擎：解析、优化、执行
- **[nimbus-kv](https://github.com/EAnge1o/nimbus-kv)** — Raft 共识的分布式 KV 存储
- **[nimbus-chain](https://github.com/EAnge1o/nimbus-chain)** — 零依赖区块链

## 💼 应用与工程

- **[ai-study-copilot](https://github.com/EAnge1o/ai-study-copilot)** — 上传课件即得带引用的 RAG 学习伴侣
- **[ai-interview-coach](https://github.com/EAnge1o/ai-interview-coach)** — AI 面试陪练：模拟面试、逐题点评与能力画像
- **[careeraid-ai](https://github.com/EAnge1o/careeraid-ai)** — AI 驱动的大学生职业规划全流程 Web 应用
- **[second-hand-trading-platform](https://github.com/EAnge1o/second-hand-trading-platform)** — 校园二手交易：单体 + 微服务双架构后端，Vue3 前端
- **[healthApp](https://github.com/EAnge1o/healthApp)** — uni-app 跨端健康管理，接入百度 AI 与豆包 LLM

## 🛠 工具

- **[star-radar](https://github.com/EAnge1o/star-radar)** — 开源趋势雷达：按「真实增速」而非总量排行，每日快照自动存档，AI 一句话中文点评
- **[nba2k27-keyboard-remap](https://github.com/EAnge1o/nba2k27-keyboard-remap)** — Go 系统级按键重映射，修复游戏内无法改键的问题
- **[AI-IDE-Agent-Prompts](https://github.com/EAnge1o/AI-IDE-Agent-Prompts)** — AI IDE Agent 提示词库
- **[bot](https://github.com/EAnge1o/bot)** — 实验性 Bot 🚧 *填充中*

---

🚧 = 填充中，敬请期待
