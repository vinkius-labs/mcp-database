# Caiyun AI Translate / 彩云小译 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/caiyun-ai-translate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Popular high-precision machine translation — translate text lists and detect languages via AI.

## Description
Empower your AI agent to orchestrate your global communication and high-precision translation with **Caiyun AI Translate** (彩云小译), one of China's most popular machine translation platforms. By connecting Caiyun to your agent, you transform complex multilingual tasks, text list processing, and technical localization into a natural conversation. Your agent can instantly translate multiple strings in a single request, provide confidence scores for translations, and support diverse language pairs including Chinese, English, Japanese, and Korean. Whether you are localizing software interfaces or translating diverse social media feeds, your agent acts as a real-time linguistic coordinator, providing accurate and context-aware results from a single, authorized source.

### What you can do

- **Batch Translation** — Translate lists of strings simultaneously to maintain context and speed.
- **Precision Mapping** — Access high-quality translations for ZH, EN, JA, and KO with dedicated tools.
- **Confidence Auditing** — Receive confidence scores for every translation to ensure data reliability.
- **Multilingual Support** — Bridge communication gaps between major Asian and Western languages.
- **Connectivity Monitoring** — Verify API connectivity and gateway status to ensure translation uptime.

### How it works

1. Subscribe to this server
2. Enter your Caiyun Interpreter Token (小译 Token)
3. Start translating your global content through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **App Developers** — automate the localization of UI strings and resource files through natural language queries.
- **Content Analysts** — translate large volumes of social media or news data directly from your AI-powered workspace.
- **Developers** — integrate professional-grade machine translation into your AI-driven daily routines.
- **Caiyun Power Users** — integrate your existing translation workflows into your AI-driven daily routines.


## Available Tools (10)
- **check_caiyun_status**: Check API connectivity
- **detect_language_via_auto**: Identify language of text
- **translate_en_to_zh**: Translate English to Chinese
- **translate_ja_to_zh**: Translate Japanese to Chinese
- **translate_ko_to_zh**: Translate Korean to Chinese
- **translate_multiple_lines**: Translate multiple text blocks
- **translate_text**: Translate text list
- **translate_to_en**: Translate to English
- **translate_to_zh**: Translate to Chinese
- **translate_zh_to_en**: Translate Chinese to English


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caiyun AI Translate / 彩云小译** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate these phrases to Chinese: 'Good morning', 'How can I help you?', 'Have a nice day'."

**🤖 AI Agent:**
> I've translated your list of phrases to Simplified Chinese using Caiyun AI. 1. '早上好' (Zǎoshang hǎo), 2. '我能帮你什么吗？' (Wǒ néng bāng nǐ shénme ma?), 3. '祝你度过愉快的一天' (Zhù nǐ dùguò yúkuài de yītiān). Would you like me to translate more strings?

---

**👤 You:**
> "Translate this Japanese note to Chinese: 'こんにちは、お元気ですか？'"

**🤖 AI Agent:**
> I've translated the Japanese text to Simplified Chinese. The translation is: '你好，你好吗？' (Nǐ hǎo, nǐ hǎo ma?). The Caiyun API performed this with high confidence. Should I check the API status for you?

---

**👤 You:**
> "Translate 'Hello' to Chinese, English, and Japanese in one go."

**🤖 AI Agent:**
> Using Caiyun's multi-translation capability, here is 'Hello': 1. Chinese: '你好', 2. English: 'Hello', 3. Japanese: 'こんにちは'. Would you like me to translate a different word into these languages?


## ❓ FAQ

**Q: How do I find my Caiyun Interpreter Token?**
Log in to the [Caiyun Open Platform](https://fanyi.caiyunapp.com/#/api), navigate to the API Token section in your dashboard to find your unique Interpreter Token.

**Q: What does 'auto2zh' mean?**
It is a direction code where 'auto' indicates automatic source language detection and 'zh' indicates Simplified Chinese as the target language. Other codes follow the [source]2[target] pattern.

**Q: Can I translate multiple lines at once?**
Yes! Use the `translate_text` or `translate_multiple_lines` tools. You can provide a comma-separated list or a JSON array of strings to be translated in a single API call.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/caiyun-ai-translate](https://vinkius.com/mcp/caiyun-ai-translate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caiyun AI Translate / 彩云小译** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `caiyun-ai-translate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caiyun AI Translate / 彩云小译** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caiyun-ai-translate": {
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
