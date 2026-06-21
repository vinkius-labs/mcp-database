# Weblate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weblate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate localization workflows via Weblate — manage projects, components, languages, and users directly from any AI agent.

## Description
Connect your **Weblate** instance to any AI agent to streamline your continuous localization and translation management through natural conversation.

### What you can do

- **Project & Component Management** — List all projects, fetch component details, and explore translation files directly from the Weblate API.
- **Language Insights** — Retrieve detailed statistics for specific languages to track translation progress and identify missing strings.
- **User & Group Administration** — Manage user profiles, list contributions, and handle group roles or administrative permissions.
- **Repository Operations** — Perform critical repository actions like pulling updates or pushing translations to keep your version control in sync.
- **Notification Control** — List and manage user notification subscriptions to stay updated on translation changes.

### How it works

1. Subscribe to this server
2. Enter your Weblate Instance URL and Personal API Token
3. Start managing your localization projects from Claude, Cursor, or any MCP-compatible client

No more switching between your IDE and the Weblate dashboard to check translation status or user permissions. Your AI acts as a localization manager.

### Who is this for?

- **Localization Managers** — quickly check project health, language coverage, and user contributions without manual reporting.
- **Developers** — trigger repository syncs and inspect component structures directly from the code editor.
- **DevOps Engineers** — automate user provisioning and group role assignments within the localization infrastructure.


## Available Tools (32)
- **add_group_admins**: Add team administrators to a group
- **add_group_roles**: Associate roles with a group
- **create_group**: Create a new group
- **create_language**: Create a new language definition
- **create_project_component**: Create a new component in a project
- **create_project**: Create a new project
- **create_role**: Create a new role with specific permissions
- **create_user**: Create a new Weblate user
- **delete_user**: Delete a user (marks inactive)
- **get_group**: Get group details (roles, projects, components)
- **get_language**: Get language details (plural formulas, aliases)
- **get_project**: Get project details
- **get_role**: Get role details and permission codenames
- **get_user**: Get detailed user information
- **list_groups**: List Weblate groups
- **get_language_statistics**: Global statistics for a language
- **list_languages**: List all languages
- **list_user_notifications**: List user notification subscriptions
- **manage_user_notifications**: Manage user notification subscriptions
- **list_project_components**: List components within a project
- **get_project_file_url**: Get the URL to download all translations as a ZIP archive
- **list_project_labels**: Manage project labels
- **list_project_languages**: Paginated statistics for all languages in a project
- **perform_repository_operation**: Perform VCS operations (push, pull, commit, reset, cleanup)
- **get_project_repository**: Overall VCS status for the project
- **list_projects**: List all projects
- **list_roles**: List roles associated with the user
- **get_root**: Get Weblate API root entry point
- **update_user**: Update user details
- **get_user_contributions**: List translations with user contributions
- **get_user_statistics**: Get user translation statistics
- **list_users**: Requires management permissions or returns self.

List Weblate users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weblate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active localization projects in Weblate."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Mobile App' (Slug: mobile-app), 'Web Dashboard' (Slug: web-dash), and 'Documentation' (Slug: docs). Which one would you like to explore?

---

**👤 You:**
> "Show me the translation statistics for the German language."

**🤖 AI Agent:**
> Fetching statistics for 'de'... The German language currently has 85% completion across all projects, with 1,200 translated strings and 150 strings requiring attention (fuzzy or untranslated).

---

**👤 You:**
> "Get detailed information for user 'johndoe'."

**🤖 AI Agent:**
> Inspecting user 'johndoe'... Full Name: John Doe, Email: john@example.com. This user is active and belongs to the 'Translators' and 'Reviewers' groups.


## ❓ FAQ

**Q: Can I check the translation progress for a specific language code?**
Yes! Use the `get_language_statistics` tool with the language code (e.g., 'fr'). The agent will return detailed metrics including translated, fuzzy, and failing strings.

**Q: Is it possible to trigger a Git pull or push from the AI?**
Absolutely. Use the `perform_repository_operation` tool. You can specify the project and component along with the operation (like 'pull' or 'push') to sync with your remote repository.

**Q: Can I manage user access and view their contributions?**
Yes. You can use `list_users` to see accounts, `get_user_contributions` to audit translation activity, and `add_group_roles` to manage permissions programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weblate](https://vinkius.com/mcp/weblate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weblate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weblate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weblate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weblate": {
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
