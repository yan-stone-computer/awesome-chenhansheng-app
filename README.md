<div align="center">

<img src="images/cover.png" width="120" style="border-radius: 24px;" alt="陈汉升" />

# 陈汉升 · 智能体对话 APP

**重生之人生导师** —— 把《我真没想重生啊》里的陈汉升装进你的手机

[![官网](https://img.shields.io/badge/官网-GitHub%20Pages-181717?style=flat-square&logo=github&logoColor=white)](https://yan-stone-computer.github.io/awesome-chenhansheng-app/)
[![平台](https://img.shields.io/badge/平台-Android%208.0%2B-3DDC84?style=flat-square&logo=android&logoColor=white)](https://github.com/yan-stone-computer/awesome-chenhansheng-app)
[![语言](https://img.shields.io/badge/语言-Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://github.com/yan-stone-computer/awesome-chenhansheng-app)
[![AI](https://img.shields.io/badge/AI-DeepSeek-4D6BFE?style=flat-square&logo=deepseek&logoColor=white)](https://www.deepseek.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

原生安卓 AI 角色扮演应用 · DeepSeek 对话 · 识图/生图（内置免费引擎） · 纯 Kotlin 开发

</div>

---

## ✨ 特性

| | 特性 | 说明 |
|---|---|---|
| 🗣️ | **陈汉升人格对话** | 口头禅、笑声、见人下菜的语气、江湖智慧，深度还原《我真没想重生啊》男主，不是冷冰冰的 AI |
| 🖼️ | **发图识图** | 截图 / 照片 / 表情包都能看；内置智谱免费引擎（GLM-4V-Flash），国内直连、零配置 |
| 🎨 | **AI 生图** | 输入栏魔法棒一键生图；内置智谱免费引擎（CogView-3-Flash），国内直连、零配置 |
| 🧠 | **剧情知识库** | 内置《我真没想重生啊》1000+ 章全文索引，聊到任何情节都能对得上原著 |
| 🗣️ | **会话记忆** | 记得你说过的事、正在烦的事，下次接着聊；清空对话记忆同步清零 |
| 📱 | **纯原生 APP** | Kotlin + Material 3 + RecyclerView + OkHttp，非网页套壳，启动快、手感顺 |
| 🔒 | **Key 只存本机** | DeepSeek Key 仅保存在手机本地，不内置、不上传、不共享 |

## 📸 界面预览

<div align="center">
  <img src="images/app-screenshot.jpg" width="280" alt="APP 界面实拍" style="border-radius: 28px; border: 1px solid rgba(212,175,55,.3);" />
  <br/>
  <sub>APP 真机界面 · 深色鎏金主题</sub>
</div>

## 🚀 快速开始（本地预览官网）

```bash
# 方式一：直接双击 index.html
# 方式二：本地静态服务
python -m http.server 8080 --directory .
# 浏览器访问 http://localhost:8080
```

## 🛠 技术栈

| 模块 | 方案 |
|---|---|
| 语言 | Kotlin 2.0 |
| UI | Material 3（深色主题）+ ViewBinding + RecyclerView |
| 对话模型 | DeepSeek（`deepseek-chat`，SSE 流式） |
| 识图引擎 | GLM-4V-Flash（智谱，内置免费、国内直连） |
| 生图引擎 | CogView-3-Flash（智谱，内置免费、国内直连） |
| 网络 | OkHttp 4.x（多轮重试 + 引擎 failover） |
| 异步 | Kotlin 协程 |
| 存储 | SharedPreferences（Key 与聊天记录，仅本机） |

## 📦 下载安装

> **v4.1.0** · 9 MB · Android 8.0+ · 内置 1000+ 章剧情知识库 · 会话记忆 · 生图/识图（内置免费国内引擎，零配置）· 无内置 Key

- 🔗 百度网盘（提取码 `t4fb`）：<https://pan.baidu.com/s/1qBZf9LpIVY7sBzOd0Q7AWg?pwd=t4fb>
- 📁 仓库镜像：`download/ChenHanshen_v4.1.0.apk`

**使用三步：**

1. **下载 APK**：通过网盘保存/下载到手机
2. **填入你的 Key**：只需填 DeepSeek Key（必填）开聊；识图、生图已内置免费引擎，零配置直接用
3. **开唠**：感情、饭局、职场、被欺负了，直说；发图也行，他眼神好使

## 📁 项目结构

```
awesome-chenhansheng-app/
├── website/                  # 官网落地页（本仓库）
│   ├── index.html            # 官网单页
│   ├── favicon.svg           # 网站图标（金色印章）
│   ├── images/               # 封面 / APP 截图 / 技能库截图
│   └── download/             # APK 镜像
└── README.md
```

## 🔧 开发与构建（APP 源码）

APP 本体为独立工程（Kotlin 原生），构建环境：JDK 17 + Android SDK 34 + Gradle 8.10.2：

```bash
cd android
JAVA_HOME="<JDK17路径>" gradle assembleRelease --no-daemon
# 产物：android/app/build/outputs/apk/release/app-release.apk
```

## 🌐 部署

官网为纯静态单页，任意静态托管可用（GitHub Pages / Vercel / CloudStudio 等）：

- 当前线上：**GitHub Pages** <https://yan-stone-computer.github.io/awesome-chenhansheng-app/>
- 更新步骤：修改 `website/` 内容 → push 到 main 分支 → Pages 自动发布

## 🙏 致谢

- 角色人格与话术体系：开源项目 [awesome-chenhansheng-app](https://github.com/yan-stone-computer/awesome-chenhansheng-app)
- 原作：小说《我真没想重生啊》（柳岸花又明）
- 对话能力：[DeepSeek](https://www.deepseek.com/) · 识图/生图：[智谱 BigModel](https://open.bigmodel.cn/)

## 📄 License

- 本站源码：MIT
- APK：个人自用，禁止商业分发
- 角色形象与小说内容版权归原作者所有，本站仅作学习交流
