<div align="center">

![Typing SVG](https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&lines=Hi+there+%F0%9F%91%8B%2C+I%27m+E%27Angelo;%E4%BB%8E%E9%9B%B6%E9%80%A0%E7%B3%BB%E7%BB%9F+%C2%B7+AI+%E5%BA%94%E7%94%A8+%C2%B7+%E5%85%A8%E6%A0%88%E5%BC%80%E5%8F%91;%E6%8A%8A%E5%A4%8D%E6%9D%82%E7%9A%84%E4%B8%9C%E8%A5%BF%E6%8B%86%E5%88%B0%E5%BA%95%E5%B1%82%E5%AE%9E%E7%8E%B0)

**AI 应用 · 全栈开发 · 从零造系统**

[![Followers](https://img.shields.io/github/followers/EAnge1o?label=Followers&style=for-the-badge&color=0e83cd&logo=github)](https://github.com/EAnge1o)
[![Profile Views](https://komarev.com/ghpvc/?username=EAnge1o&color=0e83cd)](https://github.com/EAnge1o)

</div>

---

## 🧑‍💻 关于我

- 🎓 在校学生
- 🔥 技术主线：**Agent 基础设施 / AI 应用 / 全栈**
- 🌱 正在深耕：Agent 可测试性、RAG、LLM 推理优化
- 🏁 常驻赛场：Kaggle · ARC Prize · 各类黑客松与创意开发大赛
- ⚡ 平时写小工具、打篮球 🏀、折腾新东西

---

## 🚀 旗舰项目

> 不堆仓库数量，只养能一直用的东西。三个正在长期维护的旗舰：

### [tapedeck](https://github.com/EAnge1o/tapedeck) · 给 LLM Agent 的飞行记录仪

**tapedeck** 录一次（REC ⏺），永久离线重放（PLAY ▶），精确 diff 出第一个漂移的步骤（⏩）。

> 每个做过 Agent 的人都遇到同一个夜晚：**昨天还好好的 agent，今天改了一行 prompt 就坏了。** 重跑一次要花钱，重跑十次才复现，日志里只有一坨 print。tapedeck 把整次运行录成带版本号的 JSONL；之后重放零 API 成本、逐字节确定；两个 run 一条命令 diff，直接告诉你**第几步、哪个调用、从什么值变成了什么值**。

- ⏺ **REC**：模型调用、工具调用、usage 全部记档，trace 就是本地文件，可进 git
- ▶ **PLAY**：重放 0 次 API 调用、$0.00、逐字节确定——录制即回归测试
- ⏩ **diff** 退出码直连 CI：`0` 一致 / `1` 输出漂移 / `2` 结构漂移
- 🧩 纯 Python 标准库，零依赖，不上传任何数据

![tapedeck demo: record / replay / diff](https://raw.githubusercontent.com/EAnge1o/tapedeck/main/docs/demo.svg)

### [mocktape](https://github.com/EAnge1o/mocktape) · 单文件 Mock API

**mocktape** 是前端与集成测试用的 Mock API 服务器：一份配置起一套 CRUD（INIT），录制真实接口存成卡带（REC ⏺），离线随处重放（PLAY ▶）。

> 联调第一天，后端接口还没好；联调第三天，第三方 API 限流、慢、按次收费。mocktape 让前端不再干等：`npx mocktape init` 一份 JSON 就有完整 CRUD；真实接口录一次，之后断网也能重放；404 不再只是 404——它告诉你**最像的是哪个路径、差在哪个参数**。

- 📦 一份 JSON 配置 → 完整 CRUD API，直接建立在 `node:http` 上的轻内核
- ⏺ 录制真实接口 → 可重放 cassette，测试套件里还能当库用
- 🧯 最近匹配诊断、场景切换、故障注入与延迟、实时流量 Dashboard

![mocktape in the terminal](https://raw.githubusercontent.com/EAnge1o/mocktape/main/docs/assets/terminal.gif)

### [star-radar](https://github.com/EAnge1o/star-radar) · 开源趋势雷达

**star-radar** 每天自动观测 GitHub，按「真实增速」而非总量排行，一页看懂开源世界正在发生什么。

> 总量榜告诉你谁赢过，增速榜告诉你谁正在爆发。按近 24 小时 / 7 天 / 28 天新增 Star 排序，比总量榜更早发现趋势；新锐项目自动聚成赛道，AI 一句话点评「这是什么 + 为什么火」。

- 📈 增速榜 + 新秀榜（创建 ≤ 30 天就起量）+ 黑马标记 🔥（日增速 > 3× 同语言基线）
- 🛤️ 实时赛道聚类 + AI 中文点评 ✦
- 🗄️ 每日快照存档，star 曲线随时间生长；内置 817 个真实项目种子库，开箱即用

<p align="center">
  <img src="https://raw.githubusercontent.com/EAnge1o/star-radar/main/screenshots/home.png" alt="StarRadar 首页" width="48%">
  <img src="https://raw.githubusercontent.com/EAnge1o/star-radar/main/screenshots/fresh.png" alt="StarRadar 新秀榜" width="48%">
</p>

## 🥇 Kaggle

### [Predicting-Airline-Satisfaction](https://github.com/EAnge1o/Predicting-Airline-Satisfaction) · Kaggle Playground S6E10

`✅ 已提交` 航空公司满意度预测：用固定折验证、航线特征与嵌套 OOF 堆叠，把单模型约 `0.9602` 的 AUC 提升到公开榜 **`0.96213`**，当时排名 **122 / 3142**。

- ✈️ 把 `Flight Distance` 当作航线代理，加入无标签航线画像与折内目标编码
- 🧪 固定 `StratifiedKFold` 验证面，分别保存 OOF、测试预测和提交结果
- 🧱 使用独立种子做嵌套 CV 逻辑回归堆叠，并自动筛除高相关近重复成员
- 📉 公开榜只认超出噪声的增益；最终保留 CV 主提交与 public-max 风险对冲两种不同赌注
- 📚 仓库包含方法、失败实验、公开方案复盘和可复现代码，不包含比赛数据或预测文件

### [Kaggle-Google-The-Gemma-4-Developer-Agent](https://github.com/EAnge1o/Kaggle-Google-The-Gemma-4-Developer-Agent) · Kaggle × Google — The Gemma 4 Developer Agent

`🔴 比赛中` 基于 Gemma 4 的开发者 Agent 方案，比赛进行中，赛后再上传分享。

## 🏆 比赛

### [mcd-repeat-smarter](https://github.com/EAnge1o/mcd-repeat-smarter) · 麦当劳中国程序员创意开发大赛

`🔴 参赛中` 麦麦老样子 · McD Repeat Smarter —— 基于麦当劳官方 MCP 的个性化点餐助手。起点不是菜单，是你最近的一单。

- 🍟 零 SDK 手写 MCP 客户端，35 个 Tool 里实际用 7 个
- 🧾 每次核价取官方结果，金额可查 `traceId`
- 🔒 勾选「我已核对」才提交，系统不替用户下单

### [midnight-oracle](https://github.com/EAnge1o/midnight-oracle) · 小红书小工具创意大赛

`🔴 参赛中` 镜映心 —— 离线「塔罗 + 答案之书」小工具。把抽到的牌面当成答案之书的那一页：牌给意象，一句话替你开口。

- 🌙 差异化路线：塔罗意象 × 答案之书，不预测未来、不收集问题
- 📖 264 句提示语，22 张大阿尔卡那 × 正逆位 × 6 种此刻状态
- 🔇 音效全部 Web Audio 实时合成，0 个音频资源；全程离线 0 网络请求
- 📱 严格遵循小红书小工具容器约束：单 HTML 入口、Chrome 61 兼容、交付包 1.94 MiB
- 🖼️ 1080×1440 竖版分享卡，正好小红书图文比例

> 在线体验 & 项目主页：<https://eange1o.github.io/midnight-oracle/>

## ⚡ 黑客松

### [ARC-Prize-2026-ARC-AGI-3](https://github.com/EAnge1o/ARC-Prize-2026-ARC-AGI-3) · ARC Prize 2026（ARC-AGI-3）

`🔴 比赛中` ARC-AGI-3 求解方案，比赛进行中，待上传分享。

### TruLens · 欧莱雅黑客松

`✅ 已提交` 赛题二「信任守护师 — 创造者的 AI 卫士」：面向美妆护肤种草内容的多模态真实性核验 Agent，把一条看似完整的种草帖拆开看。

- 🔍 四维可信度分析：T 账号可信度 / R 图片真实性 / U 评论区真实性 / S 文案真实性，每维独立出分 + 可解释证据链
- 🧠 多 Agent 架构：account / image / comment / text 四个分析 Agent + 融合报告 Agent，全链路带 engine trace
- 📊 自建评测框架与标注数据集（22 条样本黑盒评估），覆盖伪造与对照样本
- 🏗️ FastAPI 后端 + React 前端 + content-trust-engine 分析引擎（TruFor / FerretNet / NFA-ViT 图像取证 + DeepSeek / Qwen VL 多模态推理）

> 源码在私人仓库，如有交流意向可联系。

### [octos-arc](https://github.com/EAnge1o/octos-arc) · ARC-Bench 黑客松

`✅ 已收官` 基于 Octos 的自主软件工程 Agent：把需求文档和参考图转换成可运行的全栈 Web 应用。

- 🔁 Playwright 自测 + 修复的闭环迭代，在 ARC-Bench 的隐藏测试与成本约束下评估
- 🧬 从初赛打磨到收官共 9 个 agent bundle 演进，完整复盘沉淀在私人仓库（可私下分享）

## 🤖 AI 应用 · Agent

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

## 🛠️ 小工具

| 项目 | 一句话说明 | 技术栈 |
| --- | --- | --- |
| [nba2k27-keyboard-remap](https://github.com/EAnge1o/nba2k27-keyboard-remap) | NBA 2K27 系统级按键重映射，解决游戏内无法改键 | `Go` |
| [bot](https://github.com/EAnge1o/bot) | 实验性 Bot（挖坑中，敬请期待） | WIP |

## 🛠️ 技术栈

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-DEA584?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Vue.js](https://img.shields.io/badge/-Vue.js-42B883?style=flat-square&logo=vue.js&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
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
