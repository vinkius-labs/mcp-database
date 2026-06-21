# Apiary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apiary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your API design-first workflows via Apiary — read blueprints, publish docs, and run tests directly from your AI agent.

## Description
Connect your **Apiary** workspace to your AI agent and take full control of your API design, specification, and validation processes through natural conversation.

### What you can do

- **Read API Blueprints** — Fetch raw Markdown-based API Blueprints or Swagger files defining endpoints, methods, and parameters without leaving your editor
- **Publish Documentation** — Instantly update your Apiary projects with new markdown code. Mock servers and public documentation sync automatically
- **Run Dredd Tests** — Validate your backend implementation against the blueprint specifications using integrated tests
- **Team Management** — Query team API projects, list team members, and manage your engineering ecosystem intuitively

### How it works

1. Subscribe to this server
2. Enter your Personal Apiary Token
3. Start querying your APIs or instruct Claude/Cursor to refactor endpoints instantly

No copying and pasting back and forth to the Apiary browser editor.

### Who is this for?

- **Backend Engineers** — ask your assistant to fetch the current blueprint, write new endpoint specifications, and publish them back automatically
- **Technical Writers** — easily review and fix API documentation formatting and submit changes directly to the remote server
- **Engineering Managers** — list all active APIS under your team, oversee member permissions, and check the testing status


## Available Tools
- **list_apis**: Apiary is an API design-first platform.

List all API projects on Apiary
- **get_api**: Get the full API Blueprint source code of an Apiary API project
- **publish_blueprint**: Use with valid Markdown blueprint/Swagger.

Publish (update) the API Blueprint of an Apiary API project
- **get_me**: Get the authenticated Apiary user profile
- **list_team_apis**: List all API projects belonging to a specific Apiary team
- **list_teams**: List all teams the authenticated user belongs to on Apiary
- **get_team**: Get details of a specific Apiary team
- **list_team_members**: List all members of an Apiary team
- **run_tests**: Get or run Dredd-style API tests against an Apiary project
- **get_doc_url**: Get the documentation and mock server URLs for an Apiary API project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apiary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the API Blueprint code for my project named 'payments-gateway'."

**🤖 AI Agent:**
> Here is the raw Markdown blueprint from 'payments-gateway'. It currently has 15 endpoints categorized under 'Transactions' and 'Refunds'. How would you like me to modify it?

---

**👤 You:**
> "List all team members of the 'frontend-team' in Apiary."

**🤖 AI Agent:**
> I've fetched the member list for 'frontend-team'. There are 4 members associated with this workspace, including 1 admin and 3 regular publishers. Would you like to check what APIs this team owns?

---

**👤 You:**
> "Update my 'users-api' with this new blueprint code..."

**🤖 AI Agent:**
> I have successfully published the updated markdown code to 'users-api'. Apiary has verified the syntax to be valid Blueprint, and the mock server along with the documentation URL has been refreshed automatically.


## ❓ FAQ

**Q: Can the agent fetch the exact mock server endpoints for one of my APIs?**
Yes. You can use the `get_doc_url` capability to retrieve both the public facing documentation url and the private mock server endpoint string. Your agent can immediately use this url to simulate requests internally using other modules or tests.

**Q: Am I able to update the Blueprint markup completely through the agent?**
Absolutely. Instruct your AI agent to fetch the blueprint with `get_api`. Once read into context, prompt the agent to make your desired changes (e.g. 'Add a new POST route for user creation'). Then, instruct it to use `publish_blueprint` to upload the newly revised markdown.

**Q: How does the team feature list function mapping work?**
Apiary enables collaboration. Utilizing `list_teams`, the agent finds the slugs of your organizations. Then, using `list_team_apis`, it fetches all collaborative APIs available for that precise team. This hierarchy avoids hallucinating random endpoint repositories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apiary](https://vinkius.com/mcp/apiary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apiary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apiary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apiary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apiary": {
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
