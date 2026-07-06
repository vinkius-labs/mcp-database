# DeepL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Translate and audit text — manage multilingual communication via AI.

## Description
Empower your AI agent to orchestrate your entire multilingual workflow with **DeepL**, the world's most accurate AI translator. By connecting DeepL to your agent, you transform complex translation tasks into a natural conversation. Your agent can instantly translate text between dozens of languages, audit available language pairs, and monitor API usage without you ever touching a technical dashboard. Whether you are localized content or communicating with international teams, your agent acts as a real-time linguistic bridge, ensuring your communication is always precise and professional.

### What you can do

- **Text Auditing** — Translate text into target languages and retrieve detected source language metadata instantly.
- **Linguistic Oversight** — List all supported source and target languages to maintain a clear view of translation options.
- **Usage Intelligence** — Monitor your character count and API limits to maintain strict control over your translation budget.
- **Glossary Management** — List and query configured translation glossaries to ensure consistent brand terminology.
- **Contextual Tone Control** — Translate text enforcing strict formal, informal, or standard business tones instantly.
- **Markup Preservation** — Translate HTML elements while safely preserving tag boundaries and web structure.

### How it works

1. Subscribe to this server
2. Enter your DeepL API Key (Free or Pro)
3. Start managing your multilingual intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Managers** — monitor translation consistency and retrieve glossary metadata straight from your workflow.
- **Content Writers** — verify translated segments and audit language support for global campaigns.
- **International Teams** — perform rapid audits of project communications through natural language.
- **Operations Leads** — automate translation data querying to orchestrate cross-functional global teams smoothly.


## Available Tools (9)
- **translate_text_formal**: g., "Sie" in German, "vous" in French) suitable for business communications.

Translate text using a formal/business tone
- **translate_html_markup**: Translate HTML elements while preserving tag structure
- **translate_text_informal**: g., "du" in German, "tu" in French) suitable for casual platforms.

Translate text using an informal/casual tone
- **get_account_glossaries**: List configured translation glossaries
- **get_glossary_dictionary**: Get term mapping entries for a specific glossary ID
- **get_source_languages**: List all supported source languages for translation
- **get_target_languages**: g., EN-US, PT-BR) that DeepL can translate TO.

List all supported target languages for translation
- **get_api_usage**: Get current API usage and character limit constraints
- **translate_text_standard**: Translate text into a target language using standard tone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeepL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Hello world' into Portuguese using DeepL."

**🤖 AI Agent:**
> The translation for 'Hello world' into Portuguese is 'Olá mundo'. I've detected the source language as English. Would you like to translate more strings?

---

**👤 You:**
> "Show me all supported target languages in DeepL."

**🤖 AI Agent:**
> I've retrieved the list of 30+ supported target languages, including Spanish, French, Japanese, and Chinese. Would you like the language codes for any of them?

---

**👤 You:**
> "What is my current DeepL usage?"

**🤖 AI Agent:**
> You have used 15,000 characters out of your 500,000 monthly limit. You have 485,000 characters remaining. Would you like to check your configured glossaries as well?


## ❓ FAQ

**Q: How do I find my DeepL API Key?**
Log in to your [**DeepL account**](https://www.deepl.com/pro-account/plan), and you will find your Authentication Key under the 'Account' tab. Copy and paste it below.

**Q: Does this work with both Free and Pro API keys?**
Yes. This server automatically detects if you are using a Free key (ending in `:fx`) or a Pro key and routes requests to the correct endpoint.

**Q: Can the agent use glossaries?**
Yes. You can list your existing glossaries via the `get_glossaries` tool and identify their IDs to maintain consistency in your agent-led translations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepl](https://vinkius.com/mcp/deepl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeepL** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deepl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeepL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepl": {
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
