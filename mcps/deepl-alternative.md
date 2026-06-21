# DeepL MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepl-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deepl-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deepl-alternative-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **DeepL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepl-alternative](https://vinkius.com/mcp/deepl-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
