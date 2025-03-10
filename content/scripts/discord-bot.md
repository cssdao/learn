---
title: Discord Bot
keywords: 脚本，Discord
date: 2025.1.18
---
在 Web3 社区，**为了鼓励早期用户的参与，项目方通常会为加入 Discord 的用户授予特殊角色**（如 OG、Early Member 等）。这些角色不仅是社区的荣誉标志，还可能带来空投奖励。例如：

- **[Aligned](https://x.com/alignedlayer)** 项目曾向每位 OG 用户发放 **5000 个代币**。
- 获取 OG 的条件仅是 **在 2024 年 4 月 24 日前加入其 Discord 频道**，即可自动获得 OG 角色。

### 🎯 启发：智能撸毛工具的必要性

作为一名专业撸毛党，我深刻意识到：

- **早期身份 = 先发优势**
- **手动操作低效，自动化才是王道**

因此，我们开发了一款 **Discord 聊天机器人**，助力撸毛党高效获取各种DC 角色。

---

#### 🤖 机器人核心功能

#### ✅ **自动化互动，提升账号权重**

- **智能对话**：AI 生成自然交流内容，避免被检测为机器人。
- **定时签到**：自动签到，积累活跃积分，提高账号权重。
- **点赞 & 回复**：主动参与讨论，增加获取 OG 角色的可能性。
- **测试代币领取**：自动领取社区发放的测试代币，避免错失机会。

#### 📊 **智能策略，降低封号风险**

- **动态操作间隔**：模拟真人使用习惯，降低异常行为检测。
- **多账号管理**：支持多个账号独立运行，提高成功率。
- **代理支持**：每个账号绑定不同代理 IP，规避封禁风险。
- **日志监控**：实时查看运行情况，随时调整策略。

---

#### 🚀 快速上手指南

#### 1️⃣ **创建 `config.xlsx` 配置文件**

创建 `config.xlsx` 并填写以下字段：

|token|guildId|channelId|proxy|gapTime|
|---|---|---|---|---|
|你的Token|服务器ID|频道ID|代理IP|随机回复间隔|

📌 **示例**：

```xlsx
abc123, 987654321, 123456789, 192.168.1.1:8080, 30-60
```

---

#### 2️⃣ **获取 Discord Token**

1. 打开 Discord，按 `F12` 进入开发者工具。
2. 进入 `Network` 选项卡，搜索 `token`。
3. 复制 Token 并填入 `config.xlsx` 文件。

📌 **示例截图**：![查看教程](https://static.learn.css.show/discord_token.jpg)

---

#### 3️⃣ **获取公会 ID 和频道 ID**

1. 进入目标 Discord 服务器。
2. 右键点击服务器名称，选择 **复制 ID**，填入 `config.xlsx` 中 `guildId`。
3. 右键点击目标频道，选择 **复制 ID**，填入 `config.xlsx` 中 `channelId`。

📌 **示例截图**：![查看教程](https://static.learn.css.show/discord-id.jpg)

---

#### 4️⃣ **项目目录结构**

```
.
├── config
│   └── config.xlsx
└── 在此处运行启动命令（注意：不是 config 文件夹内）
```

---

#### 🚀 启动执行命令

```sh
docker run -e GEMINI_API_KEY=<GEMINI_API_KEY> -e TOKEN=<TOKEN> -v ./config:/app/config ghcr.io/cssdao/discord_ai_bot:latest
```

📌 **说明**：

- `<GEMINI_API_KEY>` 为 Gemini API Key，可从 [这里](https://aistudio.google.com/apikey) 购买。
- `<TOKEN>` 为程序激活码，购买后即可运行，TG 联系 @shawncvv8 获取。

---

#### 🔄 更新机器人

```sh
docker pull ghcr.io/cssdao/discord_ai_bot:latest
```

更新后，重新执行[启动命令](#启动执行命令)即可。

---

#### ⚠️ 注意事项

- **合理使用**：避免过度操作，防止账号异常。
- **保护隐私**：谨慎保管 Token 和代理 IP，防止泄露。
- **选择优质项目**：关注 OG 角色奖励较高的 Web3 项目。
- **账号隔离**：建议多账号操作，但确保账号间无明显关联。

---

✨ 借助 AI 机器人，让撸毛更智能、更高效！欢迎加入，一起探索 Web3 机会！ 🚀
