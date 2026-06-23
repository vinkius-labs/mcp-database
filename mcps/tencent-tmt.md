# Tencent TMT / 腾讯机器翻译 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-tmt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Tencent's professional machine translation — translate text and detect languages with high precision via AI.

## Description
Empower your AI agent to orchestrate your global content and multilingual communication with **Tencent TMT** (机器翻译), the premier NLP platform by Tencent Cloud. By connecting TMT to your agent, you transform complex translation tasks, language identification, and technical localization into a natural conversation. Your agent can instantly translate text between dozens of languages, automatically identify source languages, and provide enterprise-grade localized results without you ever needing to navigate the Tencent Cloud Console. Whether you are translating technical documentation or coordinating global customer support, your agent acts as a real-time linguistic coordinator, providing accurate and reliable results from a single, authorized source.

### What you can do

- **Precision Translation** — Translate text between major world languages including Chinese, English, Portuguese, Spanish, and French.
- **Language Identification** — Automatically detect the source language of any text snippet with high confidence.
- **Specialized Workflows** — Use dedicated tools for frequent language pairs (EN-ZH, ZH-EN) for faster processing.
- **Global Localization** — Bridge linguistic gaps by localizing your content for the Chinese and global markets.
- **Operational Monitoring** — Verify API connectivity and monitor service status to ensure consistent uptime.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId, SecretKey, and Region
3. Start managing your linguistic operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content & Localization Teams** — automate the translation of help articles and marketing copy through natural language queries.
- **Global Business Operations** — translate cross-border communications and market reports directly from your AI-powered workspace.
- **Developers** — integrate professional-grade machine translation into your AI-driven daily routines.
- **Tencent Cloud Power Users** — integrate your existing TMT workflows into your AI-driven daily routines.


## Available Tools (10)
- **check_tmt_status**: Check TMT API status
- **detect_language**: Detect language of text
- **translate_en_to_zh**: Translate English to Chinese
- **translate_text**: Translate text between languages
- **translate_to_chinese**: Translate text to Chinese
- **translate_to_english**: Translate text to English
- **translate_to_french**: Translate text to French
- **translate_to_portuguese**: Translate text to Portuguese
- **translate_to_spanish**: Translate text to Spanish
- **translate_zh_to_en**: Translate Chinese to English


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent TMT / 腾讯机器翻译** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate this to Portuguese using Tencent TMT: 'The system will be updated tonight at 10 PM'."

**🤖 AI Agent:**
> I've translated your sentence to Portuguese using Tencent TMT. The result is: 'O sistema será atualizado hoje à noite, às 22h'. Would you like me to translate any other notifications?

---

**👤 You:**
> "Check what language this is: '系统升级中，请稍候'。"

**🤖 AI Agent:**
> I've detected the language using Tencent TMT. The text is in **Chinese (zh)**. It means 'System upgrading, please wait'. Should I translate this into English for you?

---

**👤 You:**
> "Translate 'I am very happy to help you' from English to Simplified Chinese."

**🤖 AI Agent:**
> I've translated the phrase for you. In Simplified Chinese, it is: '我很高兴能帮助你' (Wǒ hěn gāoxìng néng bāngzhù nǐ). Should I check the status of the TMT service to ensure it is ready for more requests?


## ❓ FAQ

**Q: How do I find my Tencent Cloud SecretId and SecretKey?**
Log in to the [Tencent Cloud Console](https://console.cloud.tencent.com/), navigate to [Access Management] -> [API Key Management] to find or generate your unique SecretId and SecretKey.

**Q: Which language pairs are supported?**
TMT supports a wide range of pairs including ZH (Chinese), EN (English), PT (Portuguese), ES (Spanish), FR (French), JA (Japanese), and more. Use `auto` for the source to let TMT decide.

**Q: Does this server handle signature calculation?**
Yes! The server automatically calculates the required TC3-HMAC-SHA256 signature for every request using your provided SecretKey, ensuring secure authorized communication with Tencent Cloud TMT.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-tmt](https://vinkius.com/mcp/tencent-tmt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent TMT / 腾讯机器翻译** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tencent-tmt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent TMT / 腾讯机器翻译** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-tmt": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
