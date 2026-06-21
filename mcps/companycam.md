# CompanyCam MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/companycam)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Enable your AI agent to manage construction projects, photos, and jobsite documentation via the CompanyCam API.

## Description
Connect your AI assistant to **CompanyCam**, the photo-first documentation platform built for contractors and field service teams.

### What you can do

- **Project Browsing** — List and search projects by name, address, or status to find jobsite records quickly.
- **Photo Management** — Retrieve photos for any project, view timestamps and GPS coordinates, and check annotations.
- **Team Overview** — Check current user info, roles, and company account details.

### How it works

1. Add the CompanyCam integration to your AI toolset.
2. Provide your Access Token (found under Your Company > Account > Access Tokens).
3. Browse your jobsite data via natural language commands.

### Who is this for?

- **Contractors** — Check jobsite photos and project status without opening the mobile app.
- **Project Managers** — Get a quick overview of all active projects and their documentation.
- **Office Staff** — Pull project photos for proposals or customer reports directly from chat.


## Available Tools
- **create_project**: Create a new project in CompanyCam
- **get_current_user**: Retrieve details of the authenticated user
- **get_photo_details**: Retrieve details of a specific photo
- **get_project**: Retrieve detailed information about a specific project
- **list_all_photos**: Retrieve a list of photos across all projects in the company
- **list_project_documents**: Retrieve a list of documents attached to a project
- **list_project_photos**: Retrieve all photos associated with a specific project
- **list_projects**: Retrieve a list of projects from CompanyCam
- **list_users**: Retrieve a list of all users in your company
- **search_projects**: Quickly find a project by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CompanyCam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the first 20 projects in CompanyCam."

**🤖 AI Agent:**
> Here are your first 20 projects:
1. '123 Oak Street Roof' — 48 photos, last updated today
2. 'Downtown Office Remodel' — 125 photos, last updated yesterday
3. 'Elm Park Siding' — 22 photos, last updated 3 days ago
...
Would you like to see photos for any of these?

---

**👤 You:**
> "List all photos for project 'proj-xxxx'."

**🤖 AI Agent:**
> Project 'proj-xxxx' has 48 photos:
1. Front Exterior — taken Jan 15, 10:32 AM (GPS: 41.88, -87.63)
2. Roof Detail — taken Jan 15, 10:45 AM (GPS: 41.88, -87.63)
3. Interior Kitchen — taken Jan 15, 11:02 AM
Would you like me to filter by date or tag?

---

**👤 You:**
> "Create a new project at '456 Maple Drive'."

**🤖 AI Agent:**
> Project successfully created!
- Name: 456 Maple Drive
- Status: Active
- ID: proj-9y8z
You can now start uploading photos to this jobsite.


## ❓ FAQ

**Q: How do I get my CompanyCam Access Token?**
In the CompanyCam web app, go to **Your Company > Account > Access Tokens** and generate a new token. Copy it and paste it below.

**Q: What is a project in CompanyCam?**
A project is a container for a specific jobsite where you store photos, documents, and comments related to that location.

**Q: Can I upload photos with this integration?**
The current version focuses on browsing and retrieving project data and photos. Photo uploading may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/companycam](https://vinkius.com/mcp/companycam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CompanyCam** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `companycam` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CompanyCam** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "companycam": {
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
