<div align="center">

![Typing SVG](https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&lines=Hi+there+%F0%9F%91%8B%2C+I%27m+E%27Angelo;%E4%BB%8E%E9%9B%B6%E9%80%A0%E7%B3%BB%E7%BB%9F+%C2%B7+AI+%E5%BA%94%E7%94%A8+%C2%B7+%E5%85%A8%E6%A0%88%E5%BC%80%E5%8F%91;%E6%8A%8A%E5%A4%8D%E6%9D%82%E7%9A%84%E4%B8%9C%E8%A5%BF%E6%8B%86%E5%88%B0%E5%BA%95%E5%B1%82%E5%AE%9E%E7%8E%B0)

**从零造系统 · AI 应用 · 全栈开发**

[![Followers](https://img.shields.io/github/followers/EAnge1o?label=Followers&style=for-the-badge&color=0e83cd&logo=github)](https://github.com/EAnge1o)
[![Profile Views](https://komarev.com/ghpvc/?username=EAnge1o&color=0e83cd)](https://github.com/EAnge1o)

</div>

---

## 🧑‍💻 关于我

- 🎓 在校学生，喜欢把"看起来复杂的东西"拆到底层亲手实现一遍
- 🔥 技术主线：**系统底层 / 编译器 / 分布式** + **AI 应用**
- 🌱 正在深耕：字节码 VM、Raft/一致性、RAG、Agent、工具链
- ⚡ 平时写小工具、打篮球 🏀、折腾新东西

## 🔥 Nimbus 系统系列（从零实现）

| 项目 | 一句话说明 | 技术亮点 |
| --- | --- | --- |
| [nimbus-vm](https://github.com/EAnge1o/nimbus-vm) | 从零实现编译器 + 字节码 VM，语言名 Nimbus | 词法/语法/语义解析、46 指令 VM、闭包与 upvalue、类继承、标记-清扫 GC |
| [nimbus-git](https://github.com/EAnge1o/nimbus-git) | 从零实现 Git，兼容原生 `git` | 对象模型、DIRC index、refs、工作区快照、O((N+M)D) Myers diff |
| [nimbus-kv](https://github.com/EAnge1o/nimbus-kv) | 从零实现 Raft 一致性 KV 存储 | Raft 选举/日志复制/持久化、零运行时依赖 |
| [nimbus-infer](https://github.com/EAnge1o/nimbus-infer) | 从零实现 LLM 推理引擎，只依赖 NumPy | 字节级 BPE 分词、KV Cache、因果注意力、RoPE/GQA/SwiGLU、手写 safetensors、int8/int4 量化、GPT-2 与 LLaMA 双架构 |
| [nimbus-chain](https://github.com/EAnge1o/nimbus-chain) | 从零实现区块链 + 文档存证应用，零依赖 | 手写 secp256k1/ECDSA（RFC 6979）、SHA-256/RIPEMD-160、Merkle 证明、栈式脚本解释器（P2PKH/P2SH/多签）、PoW 与 4 倍钳制难度调整、按累计工作量分叉重组、SPV 轻客户端、asyncio P2P |

## 🏆 黑客松

几场比赛的共同点：喜欢在严苛的约束里，把一件事从头做到底。

### [mcd-repeat-smarter](https://github.com/EAnge1o/mcd-repeat-smarter) · 麦当劳中国程序员创意开发大赛　`参赛中`

我自己就是那种天天点一样东西的人，但 App 每次都让我从头选。所以这个助手的起点不是菜单，是**你最近一单**——说一句"今天不要薯饼"就够了。没用官方 SDK，手写了 MCP 客户端（35 个 Tool 里实际用 7 个）；每次核价走官方接口、金额能查到 `traceId`；下单前必须手动勾"我已核对"，系统不替任何人按确认。

### [midnight-oracle](https://github.com/EAnge1o/midnight-oracle) · 小红书小工具创意大赛　`参赛中`

做之前查了一圈，纯塔罗和纯答案之书都烂大街了。差异点是把两者缝起来：抽到哪张牌，就翻开哪一页——牌面是插图，提示语是那一页唯一的一句话。文案花的时间最多：264 句全部只说"人"、不说"事"，所以"他会不会回来"和"我该不该离职"能套上同一句。全程离线、音效靠 Web Audio 实时合成、交付包卡在 1.94 MiB——这些是小红书小工具容器逼出来的约束，倒是让它干净了不少。

> 在线体验：<https://eange1o.github.io/midnight-oracle/>

### TruLens · 欧莱雅黑客松　`已提交`

赛题二"信任守护师"。给一条看起来完整的美妆种草帖做多模态真实性核验：账号、图片、评论、文案四个维度各自出分，再合成一份带证据链的报告。最难的是评测——没有现成数据集，自己标了 22 条样本（伪造 + 对照）搭了套黑盒评估。后端 FastAPI + React 前端，图像取证用了 TruFor / FerretNet / NFA-ViT，多模态推理走 DeepSeek 和 Qwen VL。

> 源码在私人仓库，想交流可以找我。

### [octos-arc](https://github.com/EAnge1o/octos-arc) · 初版 Agent，迭代在私人仓库

用 octos 框架从零搭了一个能跑通完整闭环的 Agent：理解需求 → 写代码 → 部署 → 自己开浏览器测 → 发现问题再修。最有意思的是坚持 task-agnostic，靠 A/B 实验把一次任务的 token 消耗从 1.66 亿压到 5400 万。复盘和进阶版本在私人仓库，可以私下分享。


## 🤖 AI / Agent

| 项目 | 一句话说明 | 技术栈 |
| --- | --- | --- |
| [ai-study-copilot](https://github.com/EAnge1o/ai-study-copilot) | AI 学习助手：上传课程资料，获得带引用的 RAG 答疑、自动测验与错题分析 | `Next.js 16` `Supabase pgvector` `DeepSeek` `TypeScript` |
| [ai-interview-coach](https://github.com/EAnge1o/ai-interview-coach) | AI 面试陪练：模拟面试、逐题点评、能力画像 | `Flask` `SQLite` `LLM` |
| [AI-IDE-Agent-Prompts](https://github.com/EAnge1o/AI-IDE-Agent-Prompts) | AI IDE Agent 提示词库 | `Prompt Engineering` |

## 🌐 全栈应用

| 项目 | 一句话说明 | 技术栈 |
| --- | --- | --- |
| [second-hand-trading-platform](https://github.com/EAnge1o/second-hand-trading-platform) | 校园二手交易平台：单体 + 微服务后端，集成 AI（大学生创新项目） | `Java` `Vue3` `MySQL` |
| [healthApp](https://github.com/EAnge1o/healthApp) | 健康管理 App，集成百度 AI 与豆包大模型 | `uni-app` `Express` `MySQL` |
| [careeraid-ai](https://github.com/EAnge1o/careeraid-ai) | AI 驱动的大学生职业规划全流程 Web 应用 | `AI` `Web` |

## 🛠️ 工具

| 项目 | 一句话说明 | 技术栈 |
| --- | --- | --- |
| [nba2k27-keyboard-remap](https://github.com/EAnge1o/nba2k27-keyboard-remap) | NBA 2K27 系统级按键重映射，解决游戏内无法改键 | `Go` |
| [bot](https://github.com/EAnge1o/bot) | 实验性 Bot | WIP |

## 🛠️ 技术栈

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Vue.js](https://img.shields.io/badge/-Vue.js-42B883?style=flat-square&logo=vue.js&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Java](https://img.shields.io/badge/-Java-007396?style=flat-square&logo=java&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)

## 📊 主页数据

<p align="center">
  <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FEAnge1o&query=public_repos&style=flat-square&label=Repos&color=0e83cd" alt="Repos">
  <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FEAnge1o&query=followers&style=flat-square&label=Followers&color=0e83cd" alt="Followers">
</p>

<div align="center">

**✨ 谢谢浏览 · 如果某个项目对你有帮助，欢迎点个 ⭐**

</div>
