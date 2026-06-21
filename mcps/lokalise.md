# Lokalise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lokalise)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lokalise-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lokalise-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate translation and localization workflows via Lokalise — manage projects, keys, and translations directly from any AI agent.

## Description
Connect your **Lokalise** account to any AI agent and take full control of your translation and localization workflows through natural conversation.

### What you can do

- **Project Management** — List all translation projects, fetch detailed project metadata, and create new projects directly from the API
- **Key Management** — Query translation keys with filters by platform, tags, or filenames, plus create and update keys programmatically
- **Translation Operations** — Fetch translations for any key, add new translations with review/fuzzy flags, and manage multi-language content
- **File Import/Export** — Upload localization files (JSON, YAML, XLIFF) and generate download bundles in any supported format
- **Team & Orders** — List team members and their roles, plus inspect professional translation orders

### How it works

1. Subscribe to this server
2. Enter your Lokalise API Token
3. Start managing your localization workflows from Claude, Cursor, or any MCP-compatible client

No more jumping between the Lokalise web console and your codebase. Your AI acts as a dedicated localization coordinator.

### Who is this for?

- **Developers** — instantly create translation keys, push new strings, and pull localized files without leaving the IDE
- **Product Managers** — check translation progress across languages, review key counts, and monitor team activity
- **Localization Teams** — automate bulk uploads, generate export bundles, and manage translation orders programmatically


## Available Tools
- **add_translation**: Add translations to one or more keys
- **create_key**: Create translation keys in a Lokalise project
- **create_project**: Create a new Lokalise project
- **download_file**: Generate a download bundle of translations
- **get_project**: Get details of a specific Lokalise project
- **list_keys**: List translation keys in a Lokalise project
- **list_languages**: List languages in a Lokalise project
- **list_orders**: List translation orders in your Lokalise account
- **list_projects**: List all Lokalise projects
- **list_team_members**: List all team members in your Lokalise account
- **list_translations**: List translations for a key in a Lokalise project
- **update_key**: Update an existing translation key
- **upload_file**: Upload a localization file to a Lokalise project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lokalise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Lokalise translation projects and show their current status."

**🤖 AI Agent:**
> I've retrieved your Lokalise projects. You have 3 active projects: 'Web App' (98% localized, 5 languages), 'Mobile App' (84% localized, 4 languages), and 'Marketing Site' (100% localized, 8 languages).

---

**👤 You:**
> "Create a new translation key 'checkout.success.message' in my Web App project for the web platform."

**🤖 AI Agent:**
> Successfully created the key `checkout.success.message` in your Web App project for the web platform. It's now ready for translators to fill in across all configured languages.

---

**👤 You:**
> "Download all Portuguese (pt-BR) translations from my Mobile App project in JSON format."

**🤖 AI Agent:**
> I've generated the download bundle for Portuguese (pt-BR) translations in JSON format. The file contains 342 translated strings with 98% completion. You can download it from the provided link.


## Installation & Usage

To install and use the **Lokalise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lokalise](https://vinkius.com/mcp/lokalise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
