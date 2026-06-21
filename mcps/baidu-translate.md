# Baidu Translate / 百度翻译 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-translate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading machine translation service — translate text and detect languages via AI.

## Description
Empower your AI agent to orchestrate your global communication and multilingual content management with **Baidu Translate** (百度翻译), the premier translation platform in China. By connecting Baidu Translate to your agent, you transform complex cross-language tasks, language detection, and technical text localizations into a natural conversation. Your agent can instantly translate text between 200+ languages, automatically detect source languages, and provide high-quality localized results without you ever needing to navigate multiple translation portals. Whether you are translating e-commerce product descriptions or conducting global market research, your agent acts as a real-time multilingual assistant, providing accurate and fast results from a single, authorized source.

### What you can do

- **Multilingual Translation** — Translate text between 200+ languages including English, Chinese, Portuguese, Spanish, and French.
- **Language Detection** — Automatically identify the source language of any provided text snippet.
- **Optimized Workflows** — Use specialized tools for common language pairs like EN-ZH and ZH-EN.
- **Global Accessibility** — Bridge communication gaps by translating content into local languages with high precision.
- **System Monitoring** — Verify API connectivity and gateway status to ensure translation reliability.

### How it works

1. Subscribe to this server
2. Enter your Baidu Translate App ID and Secret Key
3. Start translating your global content through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automate the localization of articles and social media posts through natural language queries.
- **E-commerce Managers** — translate product titles and descriptions for the Chinese market directly from your workspace.
- **Developers** — integrate professional machine translation APIs into your AI-driven daily routines.
- **Baidu Power Users** — integrate your existing translation workflows into your AI-driven daily routines.


## Available Tools (10)
- **check_baidu_status**: Check Baidu Translate API status
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

Here are some examples of how you can interact with the **Baidu Translate / 百度翻译** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Hello, how are you today?' to Chinese."

**🤖 AI Agent:**
> I've translated your text to Simplified Chinese. The translation is: '你好，你今天怎么样？' (Nǐ hǎo, nǐ jīntiān zěnmeyàng?). Should I also translate the response back to English for you?

---

**👤 You:**
> "What language is this: 'Obrigado por sua ajuda'?"

**🤖 AI Agent:**
> I've detected the language using the Baidu API. The text is in **Portuguese**. It translates to 'Thank you for your help'. Would you like me to translate it into another language?

---

**👤 You:**
> "Translate this technical note from Chinese to English: '该接口支持秒级响应速度'。"

**🤖 AI Agent:**
> I've translated the technical note for you. In English, it reads: 'This interface supports second-level response speed.' Should I check the API status to ensure consistent performance for your project?


## ❓ FAQ

**Q: How do I find my Baidu Translate App ID and Secret Key?**
Log in to the [Baidu Translate Open Platform](https://api.fanyi.baidu.com/), navigate to the 'Developer Information' (开发者信息) section in your management console to find your unique App ID and Secret Key.

**Q: Which language codes are supported?**
Baidu uses standard codes like `zh` (Chinese), `en` (English), `pt` (Portuguese), `spa` (Spanish), and `fra` (French). You can use `auto` for the source language to let the API detect it automatically.

**Q: Is there a limit to text length?**
The general translation API supports up to 6000 characters per request. For extremely long documents, it is recommended to split the text into multiple smaller segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-translate](https://vinkius.com/mcp/baidu-translate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baidu Translate / 百度翻译** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baidu-translate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baidu Translate / 百度翻译** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baidu-translate": {
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
