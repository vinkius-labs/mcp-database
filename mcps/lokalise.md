# Lokalise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lokalise)
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


## Available Tools (13)
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


## ❓ FAQ

**Q: What kind of Lokalise API token do I need for this integration?**
You need a Personal Access Token from your Lokalise account. Go to your profile settings, find the API Tokens section, and generate a new token with read/write access to projects. Keep this token secure as it grants full API access to your account.

**Q: How do I add a new translation key to my Lokalise project via the AI agent?**
Use the `create_key` action with the project ID, key name (e.g., `homepage.welcome.title`), and optionally specify platforms, tags, and a description. The key will be created with the base language placeholder ready for translation.

**Q: Can I export all my translations in a specific format like JSON or YAML?**
Yes! Use the `download_file` action and specify the `format` parameter (e.g., `json`, `yml`, `xliff`, `strings`, `xml`). You can also filter by specific languages or filenames to generate targeted export bundles.

**Q: Is it possible to add translations programmatically for multiple languages at once?**
Yes. The `add_translation` action supports adding translations for one or more keys at once. You can also mark translations as fuzzy or reviewed to indicate their quality status in the workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lokalise](https://vinkius.com/mcp/lokalise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lokalise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lokalise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lokalise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lokalise": {
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
