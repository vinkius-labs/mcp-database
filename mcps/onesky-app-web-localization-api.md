# OneSky (App & Web Localization API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onesky-app-web-localization-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate app and web localization via OneSky — manage project groups, track translation progress, and handle projects directly from your AI agent.

## Description
Connect your **OneSky** localization account to any AI agent and streamline your global product expansion through natural conversation.

### What you can do

- **Project Groups** — List, create, and manage project groups to organize your localization assets across different platforms.
- **Project Management** — Create and update projects (iOS, Android, Web, etc.) and retrieve detailed metadata for each.
- **Translation Progress** — Monitor the status and progress of translations for every language enabled in your projects.
- **Language Control** — List all enabled languages within a group to ensure your target markets are covered.
- **Project Types** — Quickly identify supported project formats to ensure seamless integration with your tech stack.

### How it works

1. Subscribe to this server
2. Enter your OneSky API Key and API Secret
3. Start managing your localization workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — automate project creation and check translation status without leaving the terminal or IDE.
- **Product Managers** — track localization progress across multiple regions and manage project groups efficiently.
- **Localization Teams** — orchestrate complex translation workflows through a unified AI interface.


## Available Tools
- **create_order**: Create an order
- **create_project_group**: Create a new project group
- **create_project**: Create a new project within a project group
- **delete_file**: Delete a file from a project
- **delete_project_group**: Remove a project group
- **delete_project**: Remove a project
- **export_app_store_description**: Export translations of App Store Description in JSON
- **export_multilingual_file**: Export translations in multilingual formats
- **export_translations**: Export translations for a specific locale and source file
- **list_all_locales**: List all locales supported by OneSky
- **list_enabled_languages**: List enabled languages of a project group
- **list_import_tasks**: List import tasks for a project
- **list_orders**: List orders for a project
- **list_project_groups**: List all project groups
- **list_project_languages**: List languages of a project with translation progress
- **list_project_types**: List all available project types
- **list_projects**: List projects of a project group
- **list_uploaded_files**: List uploaded files for a project
- **make_quotation**: Make a quotation for translation
- **show_import_task**: Show details of an import task
- **show_order_details**: Show details of an order
- **show_project_group**: Retrieve details of a specific project group
- **show_project**: Retrieve details of a project
- **translation_status**: Return the progress of the translation of a specific file
- **update_project**: Update project details
- **upload_file**: Upload a file to a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneSky (App & Web Localization API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my OneSky project groups."

**🤖 AI Agent:**
> I've retrieved your project groups. You have 3 active groups: 'Marketing Site' (ID: 4567), 'iOS App' (ID: 8910), and 'Android App' (ID: 1112). Which one would you like to explore?

---

**👤 You:**
> "Show me the translation progress for project 7890."

**🤖 AI Agent:**
> For project 7890, here is the current progress: English (Base) is 100% complete, Portuguese (Brazil) is at 85%, and Spanish is at 42%. Would you like more details on a specific language?

---

**👤 You:**
> "Create a new project group named 'Global Expansion' with English as the base language."

**🤖 AI Agent:**
> Successfully created the project group 'Global Expansion' (ID: 131415) with 'en' as the base locale. You can now start adding projects to this group.


## ❓ FAQ

**Q: How can I check the translation progress for a specific project?**
You can use the `list_project_languages` tool by providing the Project ID. It will return a list of all languages associated with the project along with their respective translation progress percentages.

**Q: Can I see which project types OneSky supports through this agent?**
Yes, simply run the `list_project_types` tool. It will provide a comprehensive list of all available project formats, such as 'website', 'ios', or 'android', that you can use when creating new projects.

**Q: Is it possible to create a new project group directly from the conversation?**
Absolutely. Use the `create_project_group` tool, specifying the name and optionally the base locale. The agent will handle the API request and confirm the creation of your new group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesky-app-web-localization-api](https://vinkius.com/mcp/onesky-app-web-localization-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneSky (App & Web Localization API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `onesky-app-web-localization-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneSky (App & Web Localization API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onesky-app-web-localization-api": {
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
