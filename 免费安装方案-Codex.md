# 🦞 零成本安装小龙虾（OpenClaw）— Codex 方案

> **实测验证**：2026年3月22日，免费 ChatGPT 账号完整走通全流程。
> **适用系统**：macOS（Apple Silicon / Intel 均可）
> **费用**：0 元
> **耗时**：约 10 分钟

---

## 这个方案是什么？

上面那篇主教程用的是 Claude Code + Sub2API，每月 950 元。

这篇是**免费替代方案**——用 OpenAI 的 Codex（编程 AI 助手）代替 Claude Code 来安装小龙虾。

Codex 免费版自带完整开发环境（Node.js 等），刚好能跑小龙虾的安装命令。**你不需要懂编程，不需要自己装 Node.js，像装微信一样操作就行。**

**一句话总结：用免费 Codex 当"装修队长"，帮你把小龙虾装好。**

---

## ⚠️ 开始前确认

| 条件 | 说明 |
|------|------|
| Mac 电脑 | M 系列或 Intel 都行 |
| 能收邮件的邮箱 | 推荐 Gmail（注册 ChatGPT 用） |
| 梯子 | 稳定节点，全局 + Tun 模式 |
| 时间 | 约 10 分钟 |

> 💡 这个方案**不需要**海外手机号、信用卡、任何付费订阅。

---

## 第一步：注册免费 ChatGPT 账号（3 分钟）

1. 打开 https://chatgpt.com
2. 点「注册」，用邮箱注册
3. 验证邮箱，完成注册

注册成功后，左下角会显示「**免费版**」，侧栏会有「**Codex**」入口：

![ChatGPT 免费版主页](images/codex-tutorial/01-chatgpt-free-homepage.jpg)

---

## 第二步：下载安装 Codex App（2 分钟）

两种方式任选：

**方式 A：从 ChatGPT 侧栏进入**
- 点击左侧「Codex」→ 弹窗提示下载 → 点「下载 macOS 版」

![Codex 下载提示](images/codex-tutorial/02-codex-download-prompt.jpg)

**方式 B：直接下载**
- https://persistent.oaistatic.com/codex-app-prod/Codex.dmg

下载后打开 .dmg，把 Codex 拖到「应用程序」文件夹。

---

## 第三步：登录 Codex App（1 分钟）

1. 打开「应用程序」中的 **Codex**
2. 选择「Sign in with ChatGPT」
3. 用刚注册的免费账号登录

登录后会看到 Codex 主界面：

![Codex 主界面](images/codex-tutorial/03-codex-main-interface.jpg)

---

## 第四步：安装小龙虾（5 分钟）

在 Codex 里新建一个任务，输入：

```
请帮我安装 openclaw（小龙虾），一个 AI 助手框架。
安装命令是：npm install -g openclaw
安装完成后，运行 openclaw setup 进行初始化配置。
```

Codex 会自动执行。遇到确认提示都选「Approve」。

> 💡 Codex 自带 Node.js 环境，不需要你单独安装。

安装完后继续输入：

```
运行 openclaw setup，帮我完成配置。我需要连接 Telegram。
```

按提示操作即可。你需要准备：
- 一个 Telegram 账号
- 一个 AI 模型的 API Key（Codex 会引导你获取）

配置完成后运行 `openclaw gateway start`，你的小龙虾就活了 🦞

---

## 免费版额度够用吗？

![Codex 使用额度](images/codex-tutorial/05-codex-usage-quota.jpg)

- 免费版有**每周使用限额**，额度每周重置
- 安装小龙虾只需要几次对话，**绰绑有余**
- 安装完成后小龙虾独立运行，不依赖 Codex
- 日常维护偶尔打开 Codex 调整也够用

---

## 和主教程方案的区别

| | 主教程（Claude Code） | 本方案（Codex） |
|---|---|---|
| 费用 | ¥950/月 | 0 元 |
| 安装工具 | Claude Code | Codex App |
| AI 模型 | Claude Opus（最强） | GPT-5.4（免费版） |
| 使用限制 | Max 套餐额度内不限 | 每周有免费限额 |
| 适合谁 | 要顶配体验的人 | 先试试、预算有限的人 |

**核心区别：** 主教程花钱买的是小龙虾运行时用的 AI 模型（Claude Opus）。本方案用 Codex 只是安装工具——**小龙虾装好之后，你仍然需要一个 AI 模型来驱动它。**

如果你只是想先把小龙虾装上、体验一下再决定要不要投入，这个方案适合你。

---

## 常见问题

**Q：真的完全免费吗？**
A：安装过程完全免费。但小龙虾运行需要 AI 模型 API，有很多免费额度的选择（如 Gemini 免费版）。顶配体验需要付费（Claude Max ¥950/月）。

**Q：为什么不直接用终端安装？**
A：可以！会用终端的话直接 `npm install -g openclaw` 更快。这篇是给不熟悉命令行的朋友准备的。

**Q：装完后 Codex App 还要保留吗？**
A：小龙虾装好后独立运行，不依赖 Codex。但建议保留，以后升级维护很方便。

**Q：Windows 能用吗？**
A：目前 Codex App 只支持 macOS。Windows 用户可以用 Codex CLI（`npm i -g @openai/codex`），但需要先自己装 Node.js。

**Q：会影响电脑上已有的程序吗？**
A：不会。Codex App 和小龙虾都装在独立目录，互不干扰。

---

## 可选：Codex 设置

![Codex 设置页面](images/codex-tutorial/04-codex-settings.jpg)

- **自定义指令**：写上「请用中文回复」
- **环境**：配置运行环境
- **连接器**：可连接 GitHub

---

## 相关链接

- [主教程：完整安装路径（¥950/月顶配方案）](README.md)
- [OpenClaw 官方文档](https://docs.openclaw.ai)
- [OpenClaw GitHub](https://github.com/openclaw/openclaw)
- [Codex 官方](https://chatgpt.com/codex)
- [ChatGPT 注册](https://chatgpt.com)

---

> 📸 本教程所有截图均为 2026年3月22日实测拍摄，使用免费 ChatGPT 账号。
>
> 有问题？加微信 **ligaoxing-888**，发送「安装教程」进群交流。
