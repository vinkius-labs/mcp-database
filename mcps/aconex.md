# Aconex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aconex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage construction and engineering projects via Aconex — list projects, search directories, copy projects, and invite users directly from any AI agent.

## Description
Connect your **Aconex** account to any AI agent and take control of your construction and engineering project management workflows through natural conversation.

### What you can do

- **Project Overview** — List all projects you have access to and retrieve project logos.
- **Directory Search** — Search the Global Directory or specific project directories for users, organizations, and groups.
- **Project Administration** — Copy existing projects with detailed configurations (name, code, type, start date, etc.).
- **Team Collaboration** — Invite new users to active projects seamlessly.

### How it works

1. Subscribe to this server
2. Enter your Aconex Hostname and Authorization credentials
3. Start managing your construction projects from Claude, Cursor, or any MCP-compatible client

No more manual directory lookups or tedious project setup. Your AI acts as an automated project coordinator.

### Who is this for?

- **Project Managers** — Instantly retrieve project lists, verify project logos, and copy project templates without leaving your workspace.
- **Document Controllers & Admins** — Search global and project directories to locate organizations and users quickly.
- **Operations Leads** — Automate project duplication and user invitations to streamline onboarding.


## Available Tools
- **copy_project**: Copy an existing project
- **create_mailing_group**: Create a mailing group in a project
- **create_user**: Requires Organization Administrator permissions.

Create a new user within an organization
- **delete_mailing_group**: Delete a mailing group in a project
- **get_me**: View own user information
- **get_project_logo**: Get the logo for a specific project
- **get_register_schema**: Get the document register schema for a project
- **invite_user_to_project**: Invite a user to a project
- **list_organization_users**: Requires Organization Administrator role.

List users within an organization
- **list_projects**: List projects for the authenticated user
- **search_global_directory**: Search the Global Directory for users
- **search_project_directory**: Search a specific project directory
- **update_user_status**: Requires Organization Administrator permissions.

Enable or disable existing users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aconex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects in Aconex."

**🤖 AI Agent:**
> I have retrieved your active projects. You have access to: 'Metropolitan Highway Expansion' (ID: 849201) and 'Downtown Commercial Tower' (ID: 302948). Would you like to inspect the details of either project?

---

**👤 You:**
> "Search the global directory for users with the family name 'Smith' in the organization 'BuildCorp'."

**🤖 AI Agent:**
> Searching the Global Directory... I found 2 matching users:
1. John Smith (john.smith@buildcorp.com)
2. Sarah Smith (sarah.smith@buildcorp.com)
Would you like to invite either of them to a project?

---

**👤 You:**
> "Invite user 'usr-92018' to project 849201."

**🤖 AI Agent:**
> I've sent an invitation to user 'usr-92018' for project 849201 ('Metropolitan Highway Expansion'). They will receive a notification to join the project directory.


## ❓ FAQ

**Q: How do I list all the active construction projects I have access to?**
You can ask your AI agent to run the `list_projects` tool. It will query Aconex and return a complete list of projects associated with your authenticated account.

**Q: Can I search for users and organizations outside of my current project directory?**
Yes! Use the `search_global_directory` tool to search across the entire Aconex Global Directory using parameters like organization name, given name, family name, or email.

**Q: Is it possible to duplicate or copy an existing project template?**
Yes, you can use the `copy_project` tool. Provide the source `project_id` along with the new project's name, short name, code, type, and start date to create a copy within your organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aconex](https://vinkius.com/mcp/aconex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aconex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aconex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aconex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aconex": {
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
