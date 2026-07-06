# Dribbble MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dribbble)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Dribbble portfolio—upload shots, organize projects, and update your profile directly from your AI agent.

## Description
Connect your **Dribbble** account to any AI agent to streamline your creative workflow and portfolio management through natural conversation.

### What you can do

- **Shot Management** — List, retrieve, create, update, and delete shots using `list_user_shots`, `get_shot`, `create_shot`, `update_shot`, and `delete_shot` to keep your portfolio fresh.
- **Project Organization** — Create and manage projects with `create_project`, `list_projects`, and `update_project` to categorize your creative work effectively.
- **Profile Insights** — Access your authenticated user details, bio, and team associations via `get_user`.
- **Attachments** — Add or remove high-resolution attachments for your shots using `create_attachment` and `delete_attachment` (requires Pro/Team membership).
- **Job Tracking** — Manage job-related data and updates directly through `create_job`, `update_job`, and `get_job` tools.

### How it works

1. Subscribe to this server
2. Enter your Dribbble Personal Access Token
3. Start managing your creative assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers** — upload and update shots without leaving your design environment or code editor.
- **Creative Directors** — organize team projects and review portfolio statuses via natural language.
- **Marketing Teams** — quickly retrieve assets and metadata for social media or campaign planning.


## Available Tools (15)
- **create_shot**: Requires upload scope. Note: Video shot creation is not supported via API.

Create a new shot
- **delete_attachment**: Requires upload scope.

Delete an attachment
- **delete_project**: Delete a project
- **delete_shot**: Requires upload scope.

Delete a shot
- **get_job**: Note: Requires a special token.

Show a job
- **get_shot**: Get a specific shot
- **get_user**: Get the authenticated user
- **list_projects**: List projects
- **list_user_shots**: List the authenticated user’s shots
- **create_attachment**: Requires upload scope and Pro/Team membership.

Create an attachment for a shot
- **create_job**: Note: Requires a special token. Contact Dribbble for partnership.

Create a job
- **create_project**: Create a new project
- **update_job**: Note: Requires a special token.

Update a job
- **update_project**: Update a project
- **update_shot**: Requires upload scope.

Update an existing shot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dribbble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve my Dribbble profile information."

**🤖 AI Agent:**
> I've accessed your profile. You are logged in as 'CreativeMind' (ID: 987654). Your bio states 'UI/UX Designer based in London' and you are currently associated with the 'DesignStudio' team.

---

**👤 You:**
> "List the shots I have currently published."

**🤖 AI Agent:**
> I found 3 shots on your profile: 'Mobile App Dashboard', 'Logo Exploration', and 'Dark Mode UI'. Would you like to see the details for any of these?

---

**👤 You:**
> "Create a new project called 'Brand Identity 2024'."

**🤖 AI Agent:**
> Project 'Brand Identity 2024' has been successfully created. You can now start adding shots to this project to organize your branding work.


## ❓ FAQ

**Q: Can I upload a new design to Dribbble using this tool?**
Yes! Use the `create_shot` tool. You can provide an image URL or file data, along with a title and description, to publish a new shot to your profile instantly.

**Q: How do I organize my work into different collections?**
You can use the `create_project` and `list_projects` tools to manage your Dribbble projects, allowing you to categorize your shots and keep your portfolio organized.

**Q: Is it possible to add high-resolution files to my shots?**
Yes, if you have a Pro or Team account, you can use the `create_attachment` tool to add files (up to 10MB) to any of your existing shots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dribbble](https://vinkius.com/mcp/dribbble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dribbble** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dribbble` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dribbble** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dribbble": {
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
