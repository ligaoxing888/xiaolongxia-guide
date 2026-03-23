# 🦞 （真的是）全网最简单+零成本+高效安装小龙虾（OpenClaw）方案（gpt版）

> **实测验证**：2026年3月22日，免费 ChatGPT 账号完整走通全流程。
> **适用系统**：macOS（Apple Silicon / Intel 均可）
> **费用**：0 元
> **耗时**：约 10 分钟

---

## 这个方案是什么？

之前那篇主教程用的是 Claude Code + Sub2API，每月 950 元

这篇是**免费替代方案**——用 OpenAI 的 Codex（编程 AI 助手）代替 Claude Code 来安装小龙虾。

Codex 免费版自带完整开发环境（Node.js 等），刚好能跑小龙虾的安装命令。**你不需要懂编程，不需要自己装 Node.js，像装微信一样操作就行。**

---

## ⚠️ 开始前确认

| 条件 | 说明 |
|------|------|
| Mac 电脑 | M 系列或 Intel 都行 |
| 能收邮件的邮箱 | 推荐 Gmail（注册 ChatGPT 用） |
| 科学上网 | 稳定节点，（注册 ChatGPT 必须） |
| 时间 | 约 20 分钟 |

---

## 第一步：注册免费 ChatGPT 账号（3 分钟）

1. 打开 https://chatgpt.com
2. 点「注册」，用邮箱注册
3. 验证邮箱，完成注册

注册成功后，左下角会显示「**免费版**」，侧栏会有「**Codex**」入口：

![ChatGPT 免费版主页](images/codex-tutorial/01-chatgpt-free-homepage.jpg)

---

## 第二步：下载安装 Codex App（2 分钟）

1. 点击 ChatGPT 左侧「Codex」
2. 弹窗提示下载应用，点「下载 macOS 版」
3. 下载后打开 .dmg，把 Codex 拖到「应用程序」文件夹

![Codex 下载提示](images/codex-tutorial/02-codex-download-prompt.jpg)

---

## 第三步：登录 Codex App（1 分钟）

1. 打开「应用程序」中的 **Codex**
2. 选择「Sign in with ChatGPT」
3. 用刚注册的免费账号登录

![Codex 主界面](images/codex-tutorial/03-codex-main-interface.jpg)

---

## 第四步：用 Codex 安装小龙虾（5 分钟）

在 Codex 里新建一个任务，输入：

```
请帮我安装 openclaw（小龙虾），一个 AI 助手框架。
安装命令是：npm install -g openclaw
安装完成后，运行 openclaw setup 进行初始化配置。
```

Codex 会在它自己的界面里自动执行所有命令。遇到确认提示都选「Approve」。

安装完成后，继续在 Codex 里告诉它你想连接哪个聊天平台：

```
帮我配置小龙虾连接 [你选的平台]，引导我完成。
```

> 💡 整个安装和配置过程都在 Codex 里完成，你不需要打开终端，也不需要自己敲任何命令。

全部配置完成后，Codex 会帮你运行 `openclaw gateway start`——你的小龙虾就活了 🦞

小龙虾支持 20+ 聊天平台。推荐两个：
- **Telegram**：体验最好，功能最全，（需要海外手机号注册）
- **飞书**：国内直接注册，零门槛，适合没有海外手机号的朋友
- **微信**：正好昨天刚刚微信官宣了，可以接入，但我还没有实测，准备先观望一下，毕竟怕被封呀，哈哈

---

## 免费版额度够用吗？

![Codex 使用额度](images/codex-tutorial/05-codex-usage-quota.jpg)

- 免费版有**每周使用限额**，额度每周重置
- 安装小龙虾只需要几次对话，**绑绑有余**
- 装好后小龙虾独立运行，不依赖 Codex
- 日常维护偶尔打开 Codex 调整也够用

---

## 两个方案对比

| | Codex 方案（本篇） | 主教程方案 |
|---|---|---|
| **费用** | 0 元 | ¥950/月 |
| **安装门槛** | 不需要海外手机号和信用卡 | 需要海外手机号 + 信用卡/Apple Store |
| **安装耗时** | 约 10 分钟 | 约 3 小时 |
| **AI 模型** | GPT-5.4（模型是第二梯队） | Claude Opus（目前最强） |
| **使用限额** | 每周有免费限额，重度使用会碰天花板 | Max 套餐额度充裕 |
| **适合谁** | 先试试、预算有限 | 要顶配体验、长期使用 |

**建议：** 想先试试小龙虾是什么感觉，用 Codex 方案零成本上手。体验好了、确定要长期用，再升级到主教程的顶配方案。

---

## 常见问题

**Q：真的完全免费吗？**
A：安装过程完全免费。小龙虾装好后需要 AI 模型来驱动，GPT 免费版有免费额度可以先用着。如果想要更顶级的体验（Claude Opus），就需要付费订阅，具体看主教程。

**Q：装完后 Codex App 还要保留吗？**
A：小龙虾装好后独立运行，不依赖 Codex。但建议保留，以后升级维护很方便。

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
- [Codex 官方](https://chatgpt.com/codex)

---

> 📸 本教程所有截图均为 2026年3月22日实测拍摄，使用免费 ChatGPT 账号。
>
> 有问题？加微信 **ligaoxing-888**，发送「安装教程」进群交流。
