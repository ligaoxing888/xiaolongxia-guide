# （应该是）全网最简单且高效的 OpenClaw（小龙虾）安装路径

作者：高兴
适用人群：编程零基础、有梯子、想把 AI 真正用起来的朋友

---

## 写在前面

我是文科生、ENFJ、编程完全零基础。

花了 3 天，把小龙虾（OpenClaw）从 0 到 1 用起来了。

身边挺多人跟我一样零基础，信息又太多太乱。所以把完整路径整理出来，让跟我一样的人少走弯路。

小龙虾跟前面所有 AI 工具都不一样——脑子好、态度诚恳、啥都能干，现实中这样的人稀缺得可怕。按这个教程，不出特殊情况，最多 3 小时搞定。

这个思路来自生财一篇帖子，非常认可这种理念：
https://articles.zsxq.com/id_mwwwwcf6sq94.html

---

## 为什么选这条路

**不用套壳工具**
一开始套壳，这辈子都要被别人套着。搞投资的我，不喜欢被套牢的感觉。

**本地安装而不是云端服务器**
想要一开始尽可能无卡点、随时能折腾各种可能性。本地还有个好处：文件随手可用，基因报告存在电脑上，龙虾直接读取，不用先上传到什么平台。

**选这条路径**
先装 Claude Code，让它帮我搞定后面所有事。

**本地 Mac + Claude Code + Claude Max 会员 + Telegram 闭环**——这是我认为目前最优的路径。

---

## 开始前准备好这些

| 工具 | 说明 |
|------|------|
| Mac 电脑 | M 系列或 Intel 都可以 |
| iPhone | 充值 Claude 订阅需要在手机端操作 |
| 梯子 | 需要稳定，设置**全局 + Tun 模式**，推荐 cordc.net |
| 备用 AI | Claude.ai / ChatGPT / 豆包，遇到问题随时问 |
| 时间 | 约 3 小时 |

---

## 第一步：安装 Node.js

Claude Code 需要 Node.js 才能运行，先装这个"引擎"，没有它就跑不起来。

下载地址：https://nodejs.org/en/download/
推荐下载 **LTS 版本**，下载后直接双击安装。

安装完成后，打开终端验证：
```bash
node --version
```
看到版本号（如 `v20.x.x`）即安装成功。

> 怎么打开终端？Command + 空格，输入"终端"，回车。

---

## 第二步：安装 Claude Code

参考 3D 的视频教程，是我看过最简单、最不容易出问题的：
https://www.youtube.com/watch?v=Eq7VqmZCLQw

在终端粘贴以下命令，按回车：
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

等几分钟。遇到任何问题，截图发给备用 AI，让它告诉你下一步怎么做。

完成后在终端输入 `claude`，看到启动界面，就成功了。

---

## 第三步：给 Claude Code 充值

选择 **Claude 官方订阅**——身边朋友实测官方订阅更省 token，用的是最好的模型。

充值步骤：
1. iPhone 下载 **Claude App**
2. 用 Gmail 邮箱注册账号
3. 点击左下角账户头像
4. 选套餐：**Max（$125/月）**——我选的，想尽兴搞 😄
5. 按提示完成支付

**⚠️ 注意：** 走的是 Apple 支付，Apple ID 里必须有余额或绑定了可用的信用卡。没有余额先去 App Store → 点头像 → 充值账户。

---

## 第四步：安装小龙虾（OpenClaw）

这是最关键的一步，也是最轻松的一步。

装好 Claude Code 之后，打开它，直接说：

> 我要在这台电脑上安装 OpenClaw，帮我完成安装和配置。安装命令是：`curl -fsSL https://openclaw.ai/install.sh | bash`

然后等它干完。

**这就是这个方案的核心理念：用 AI 装 AI。**
你不需要懂代码，只需要会说话。遇到报错，把错误信息扔给 Claude Code，让它解决。

---

## 第五步：接入模型——推荐 Sub2API 方案

安装好小龙虾之后，需要配置模型。推荐 **Sub2API 方案**，比直接用 Claude 官方账户更稳定、更不容易封号。

Sub2API 开源项目：https://github.com/Wei-Shaw/sub2api

操作方式：把下面这篇冰糖橙的教程和 Sub2API 项目链接发给 Claude Code，告诉它"按照这个方案帮我配置 Sub2API"，它会自动读懂并完成配置：
https://mp.weixin.qq.com/s/s7xzFbnaxE_BVZB2vLgvcA

最终接入的模型是 **Claude Opus**——目前最强，思考质量明显高于其他版本，强烈推荐。

---

## 第六步：配置 Telegram 机器人

装好小龙虾之后，通过 Telegram 跟它对话。

**为什么选 Telegram？**
实测最清爽、最方便。飞书需要很多额外设置，直接选最少阻力的方案。

**这一步怎么配置？继续用 Claude Code！**

具体步骤：
1. 下载 Telegram 桌面版：https://desktop.telegram.org/
2. 在 Telegram 找 `@BotFather`，发送 `/newbot`，创建机器人，保存 token
3. 把 token 告诉 Claude Code，让它完成所有配置

---

## 搭建完成后，你拥有什么

- 通过 Telegram 随时对话的 AI 助手
- 可以扩展成多个专用窗口（健康、财富、学习……），同时并行处理多个任务
- 所有窗口共享记忆，不需要重复交代背景
- GitHub 自动备份，数据永远不丢

---

## 常见问题

**零基础真的能搞定吗？**
能。我就是活生生的例子。中间遇到报错，全部扔给 Claude Code 让它解决。

**梯子有什么要求？**
任何稳定的梯子都行，关键是设置**全局 + Tun 模式**，否则容易出网络问题。我用的是 cordc.net。

**遇到看不懂的报错怎么办？**
截图或复制文字，直接发给 Claude Code，让它告诉你怎么做。这是最快的方式。

**为什么不直接用套壳工具？**
套壳工具的天花板，是套壳厂商给你划定的。用原版，你的上限是你自己的想象力。

---

## 参考来源

- 生财帖子，核心理念来源：https://articles.zsxq.com/id_mwwwwcf6sq94.html
- Claude Code 安装视频（3D 出品）：https://www.youtube.com/watch?v=Eq7VqmZCLQw
- 了解 Claude Code 的形态：https://www.youtube.com/watch?v=lOcAV1B0PNs
- 冰糖橙教程，Sub2API 配置参考：https://mp.weixin.qq.com/s/s7xzFbnaxE_BVZB2vLgvcA
- Sub2API 开源项目：https://github.com/Wei-Shaw/sub2api
- 梯子推荐：cordc.net（全局 + Tun 模式）

---

具体细节、遇到的坑、更深的玩法，欢迎来找我讨论：

- **Web3 社群【群星闪耀】**（我和小鑫共同运营）：适合有 Web3 背景、想深度折腾的朋友
- **【高兴同行圈】**：如果你是女生，习惯投资，26 年准备折腾 AI，欢迎来这里一起冲

期待和大家一起，把这片虾塘承包起来 🦞

*ps：技术小白自我感觉不错，如果有不妥的地方，还请指出，谢谢。*
