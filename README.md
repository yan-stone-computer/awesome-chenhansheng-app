# 陈汉升 · 智能体对话 APP 官网

「陈汉升 · 重生之人生导师」——和《我真没想重生啊》男主陈汉升唠嗑的原生安卓 APP 的官方落地页。

- 在线预览：https://633f3581a5354fcb9761ad8fe8b7d50a.gz3.agentos-app.net
- APP 本体：原生 Android（Kotlin + Material 3），DeepSeek 对话 + 多引擎识图

---

## 页面内容

| 区块 | 说明 |
|------|------|
| Hero | 品牌封面、标语、下载入口、版本信息 |
| 为什么聊 | 四大特性：陈汉升人格 / 发图识图 / 纯原生 APP / Key 只存本机 |
| 界面预览 | APP 实拍截图（手机框展示） |
| 开源驱动 | 人格技能库 awesome-chenhansheng-skill 展示与 GitHub 入口 |
| 下载安装 | APK 下载卡片 + 三步安装说明 |

设计风格：深色鎏金（`#0D1512` × `#D4AF37`），与 APP 内界面一致；图标为内联 SVG（Feather 风格，MIT 协议），无图片字体依赖。

## 快速预览

纯静态页面，任选其一：

```bash
# 方式一：直接双击 index.html 打开
# 方式二：起本地静态服务
python -m http.server 8080 --directory .
# 浏览器访问 http://localhost:8080
```

## 目录结构

```
website/
├── index.html                 # 官网单页（内联 CSS）
├── README.md
├── images/
│   ├── cover.png              # 小说封面（Hero 展示）
│   ├── app-screenshot.jpg     # APP 实拍界面截图
│   └── github-skill.png       # 开源技能仓库截图
└── download/
    └── ChenHanshen_v2.1.2.apk # APK 安装包（49MB, Android 8.0+）
```

## APK 发布建议

- 当前版本：**v2.1.2**（49MB，Android 8.0+，支持识图，无内置 Key）
- `download/` 内的 APK 可直接被页面下载按钮引用
- 推荐改用 **GitHub Releases** 发布 APK：页面按钮指向 Releases 下载地址，避免二进制文件长期占据仓库体积
- 更换新版本时：替换 `download/` 下的 APK 并同步修改 `index.html` 中的版本号、大小等文案

## 修改与部署

1. 编辑 `index.html`（文案、截图、下载链接等）
2. 重新部署到任意静态托管（CloudStudio、GitHub Pages、Vercel 等均可）
3. 部署平台示例（CloudStudio）：选择本目录上传，即可获得公网访问链接

## 素材来源

- `app-screenshot.jpg`：陈汉升 APP 真机界面截图
- `github-skill.png`：开源技能仓库页面截图
- `cover.png`：小说《我真没想重生啊》封面

## 致谢

- 角色人格与话术体系：开源技能库 [awesome-chenhansheng-skill](https://github.com/yan-stone-computer/awesome-chenhansheng-skill)
- 原作：小说《我真没想重生啊》（柳岸花又明）

## License

- 本站源码：MIT
- APP 安装包：个人自用，请勿用于商业分发
- 角色形象与小说内容版权归原作者所有，本站仅作学习交流
