# DeepL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepl-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Translate text between 30+ languages with neural machine translation that captures nuance and tone better than generic engines.

## Description
Connect your **DeepL** account to any AI agent and access neural machine translation through natural conversation.

### What you can do

- **Text Translation** — Translate text into 30+ languages with optional formality control (formal, informal, or default)
- **Glossary-Powered Translation** — Apply custom glossaries to ensure consistent terminology across translations
- **Glossary Management** — Create, list, inspect, and delete custom glossaries with TSV term pairs
- **Language Discovery** — List all supported source and target languages, and glossary language pair combinations
- **API Usage Monitoring** — Track character count consumed, remaining quota, and billing period
- **Document Translation** — Monitor the progress of submitted document translations

### How it works

1. Subscribe to this server
2. Enter your DeepL API Key from your account dashboard
3. Start translating from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Teams** — translate marketing copy, product descriptions, and documentation with consistent terminology via glossaries
- **Content Creators** — translate blog posts and social media content with appropriate formality for each market
- **Developers** — integrate high-quality translation into AI workflows and monitor API consumption


## Available Tools (14)
- **create_glossary**: Create a glossary
- **delete_glossary**: Delete a glossary
- **get_document_status**: Check document translation status
- **get_glossary_entries**: Get glossary entries
- **get_glossary**: Get glossary details
- **get_usage**: Check API usage
- **list_glossaries**: List glossaries
- **list_glossary_language_pairs**: List glossary language pairs
- **list_source_languages**: List source languages
- **list_target_languages**: List target languages
- **translate_formal**: Translate with formal tone
- **translate_informal**: Translate with informal tone
- **translate_text**: Translate text
- **translate_with_glossary**: Translate using glossary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeepL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Welcome to our platform. We look forward to working with you.' into German (formal) and Brazilian Portuguese (informal)."

**🤖 AI Agent:**
> German (formal): 'Willkommen auf unserer Plattform. Wir freuen uns auf die Zusammenarbeit mit Ihnen.' Brazilian Portuguese (informal): 'Bem-vindo à nossa plataforma. Estamos ansiosos para trabalhar com você.' The formal version uses 'Ihnen' (Sie-form) while the informal Portuguese uses 'você' instead of 'o senhor'. Would you like to create a glossary for consistent terminology or translate more content?

---

**👤 You:**
> "Create a glossary for EN→FR with our brand terms and then translate a marketing paragraph using it."

**🤖 AI Agent:**
> Glossary created! ID: gl_8a4f2c, Name: 'Brand Terms EN-FR', Source: EN, Target: FR, Entries: 5 term pairs. Terms mapped: 'Dashboard' → 'Tableau de Bord', 'Workspace' → 'Espace de Travail', 'Insights' → 'Analyses', 'Onboarding' → 'Intégration', 'Workflow' → 'Flux de Travail'. Now translating with glossary... Result: 'Découvrez notre nouveau Tableau de Bord avec des Analyses en temps réel. L'Intégration est simplifiée grâce à notre Flux de Travail guidé dans votre Espace de Travail.' All 5 glossary terms were applied consistently.

---

**👤 You:**
> "Check my DeepL API usage and list all available target languages."

**🤖 AI Agent:**
> API Usage: 142,800 of 500,000 characters used (28.6%). Remaining: 357,200 characters. Plan: DeepL API Free. Billing period resets: May 1, 2025. Target languages available (31): BG (Bulgarian), CS (Czech), DA (Danish), DE (German), EL (Greek), EN-GB, EN-US, ES (Spanish), ET (Estonian), FI (Finnish), FR (French), HU (Hungarian), ID (Indonesian), IT (Italian), JA (Japanese), KO (Korean), LT (Lithuanian), LV (Latvian), NB (Norwegian), NL (Dutch), PL (Polish), PT-BR, PT-PT, RO (Romanian), RU (Russian), SK (Slovak), SL (Slovenian), SV (Swedish), TR (Turkish), UK (Ukrainian), ZH (Chinese). Languages with formality support: DE, FR, ES, IT, NL, PL, PT-BR, PT-PT, RU, JA.


## ❓ FAQ

**Q: Can I control the formality of translations (formal vs. informal)?**
Yes! Use `translate_formal` for professional communications (e.g., contracts, official correspondence) or `translate_informal` for casual content (e.g., social media, chat). The standard `translate_text` tool also accepts an optional formality parameter ('more', 'less', or 'default'). Note: formality control is available for select target languages including DE, FR, ES, PT-BR, and others.

**Q: Can I create custom glossaries to ensure consistent terminology?**
Yes. Use `create_glossary` with a name, source language, target language, and TSV entries (tab-separated source→target pairs). Then use `translate_with_glossary` to apply the glossary during translation. Use `list_glossaries` to see all glossaries, `get_glossary_entries` to inspect term pairs, and `list_glossary_language_pairs` for supported combinations.

**Q: How does DeepL authentication differ from standard Bearer tokens?**
DeepL uses a custom Authorization header format: `DeepL-Auth-Key YOUR_KEY` (not Bearer). Your API key is generated from the DeepL account dashboard. Free accounts use `api-free.deepl.com`, while Pro accounts use `api.deepl.com`. Use `get_usage` to check your current character consumption and plan limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepl-alternative](https://vinkius.com/mcp/deepl-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `deepl-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeepL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepl-alternative": {
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
