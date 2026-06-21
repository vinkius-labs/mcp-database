# Phrase (Software Localization API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phrase-software-localization-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/phrase-software-localization-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/phrase-software-localization-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage software localization projects, locales, and translation keys directly through the Phrase API.

## Description
Connect your **Phrase** account to any AI agent to streamline your software localization workflows. This MCP server allows you to manage projects, locales, and translation keys using natural language.

### What you can do

- **Project Management** — List, create, update, and delete localization projects directly from your agent.
- **Locale Control** — Manage target languages (locales) for each project, including setting defaults and main languages.
- **Key Management** — List and create translation keys to keep your codebase and Phrase in sync without leaving your editor.
- **Detailed Inspection** — Fetch specific details for projects and locales to understand your localization status.

### How it works

1. Subscribe to this server
2. Enter your Phrase Access Token
3. Start localizing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Create translation keys and manage locales directly from the IDE while coding.
- **Localization Managers** — Quickly list projects and check locale configurations without the Phrase web UI.
- **Product Teams** — Automate the creation of new localization projects for new features.


## Available Tools
- **create_key**: Create a new translation key
- **create_locale**: Create a new locale in a project
- **create_project**: Create a new localization project
- **create_translation**: Create a new translation
- **delete_key**: Delete a key
- **delete_locale**: Delete a locale
- **delete_project**: Delete a project
- **download_file**: Download translations in a specific format
- **get_key**: Get details for a specific key
- **get_locale**: Get details for a specific locale
- **get_project**: Get details for a specific project
- **list_keys**: List translation keys for a project
- **list_locales**: List locales for a project
- **list_projects**: List all localization projects
- **list_translations**: List translations for a project
- **update_key**: Update an existing key
- **update_locale**: Update an existing locale
- **update_project**: Update an existing project
- **update_translation**: Update an existing translation
- **upload_file**: Upload a localization file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phrase (Software Localization API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Phrase localization projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have 'Mobile App' (ID: proj_abc123) and 'Web Dashboard' (ID: proj_xyz789). Which one would you like to manage?

---

**👤 You:**
> "Show me the locales configured for project proj_abc123."

**🤖 AI Agent:**
> For project proj_abc123, I found 3 locales: English (en-US, default), German (de-DE), and Spanish (es-ES).

---

**👤 You:**
> "Create a new translation key named 'login.button.submit' in project proj_abc123."

**🤖 AI Agent:**
> Successfully created the translation key 'login.button.submit' in project proj_abc123.


## Installation & Usage

To install and use the **Phrase (Software Localization API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phrase-software-localization-api](https://vinkius.com/mcp/phrase-software-localization-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
