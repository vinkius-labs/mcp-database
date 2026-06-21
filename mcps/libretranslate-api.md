# LibreTranslate API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/libretranslate-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/libretranslate-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/libretranslate-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Translate and detect text — audit languages via AI.

## Description
Empower your AI agent to orchestrate your entire localization and language auditing workflow with the **LibreTranslate API**, the specialized source for free and open-source translation data. By connecting LibreTranslate to your agent, you transform complex translation searches into a natural conversation. Your agent can instantly translate text between dozens of languages, audit language detection confidence, and query supported language metadata without you ever touching a translation portal. Whether you are conducting regional content research or managing multilingual documentation, your agent acts as a real-time linguistic consultant, ensuring your data is always expressive and precise.

### What you can do

- **Translation Auditing** — Submits high-resolution text for translation and maintain a clear view of semantic distribution across target languages.
- **Detection Oversight** — Audit the primary language of any text string to understand the linguistic reach of your content instantly.
- **Language Discovery** — Browse all supported languages in the global catalog to identify relevant stylistic markers for your localized projects.
- **Linguistic Intelligence** — Retrieve unique language codes and names to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your translation research workflow is always operational.

### How it works

1. Subscribe to this server
2. Optional: Enter your LibreTranslate API Key or custom instance URL
3. Start managing your linguistic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Editors** — monitor translation trends and retrieve fresh linguistic metadata straight from your workflow.
- **Developers** — verify language support and audit localized strings without manual searching.
- **Content Managers** — perform rapid audits of language detection and identify relevant markers through natural language.
- **Operations Leads** — automate linguistic data querying to orchestrate cross-functional localization teams smoothly.


## Available Tools
- **check_api_status**: Check if the LibreTranslate service is operational
- **detect_language**: Detect the language of a specific text string
- **list_supported_languages**: List all languages supported by the LibreTranslate instance
- **translate_text**: Translate text from one language to another using LibreTranslate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LibreTranslate API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Hello world' from English to Portuguese using LibreTranslate."

**🤖 AI Agent:**
> I've translated the text for you! 'Hello world' in Portuguese is identified as 'Olá mundo'. Would you like the full JSON response or a different target language audit?

---

**👤 You:**
> "Detect the language of the text 'C'est la vie'."

**🤖 AI Agent:**
> I've analyzed the text! It is identified as French (fr) with a confidence score of 99%. I can provide the full metadata list of supported languages if you'd like to confirm.

---

**👤 You:**
> "List all languages supported by LibreTranslate."

**🤖 AI Agent:**
> I've retrieved the language catalog! There are dozens of languages supported, including English, Spanish, French, and Chinese. I can help you translate text between any of these thematic markers.


## Installation & Usage

To install and use the **LibreTranslate API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/libretranslate-api](https://vinkius.com/mcp/libretranslate-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
