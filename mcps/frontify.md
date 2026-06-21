# Frontify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frontify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Manage digital assets and brand guidelines via Frontify — list workspace projects and assets, handle metadata, audit brand portals, and manage users directly from any AI agent.

## Description
Connect your **Frontify** account to any AI agent and take full control of your digital asset management (DAM), brand guidelines, and collaborative workspaces through natural conversation.

### What you can do

- **Workspace Project Orchestration** — Enumerate explicitly registered project schemas and gather required IDs to browse and discover collaborative workspaces natively
- **Asset Lifecycle Management** — Retrieve detailed metadata for project assets and perform structural extraction of properties driving active media limits flawslessly
- **Brand Guideline Discovery** — Identify precise active arrays spanning rented documentation trees, identifying where strict UI/UX constraints and brand rules are registered
- **Metadata Mutation** — Update global asset boundaries by substituting attributes like titles and descriptions securely through GraphQL mutation logic
- **Media Content Oversight** — Analyze specific global boundaries iterating through brands to discover exact tenant separations inside a single account
- **Identity & User Management** — Retrieve the exact structural matching verifying identity schemas and invite new users directly into designated project workspaces securely
- **Digital Asset Purging** — Irreversibly vaporize explicit app nodes to remove media assets and separating limits pulling items offline flawlessly
- **Custom GraphQL Execution** — Identify bounded routing spaces inside the headless Frontify DAM utilizing native GraphQL strings for advanced structural queries

### How it works

1. Subscribe to this server
2. Enter your Frontify Domain and Access Token (found in your Frontify Account Settings)
3. Start managing your brand assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Brand Managers & Designers** — search for assets and organize project folders without manual DAM navigation
- **Content Marketers** — quickly look up brand guidelines and update asset metadata using natural language conversation
- **Creative Directors** — audit brand portals and verify team access to specific project workspaces in real-time
- **Developers** — test and debug GraphQL queries and verify digital asset schemas through natural conversation


## Available Tools (10)
- **wipe_media_asset**: Irreversibly vaporize explicit App nodes dropping live Database bytes
- **execute_graphql_payload**: Identify bounded routing spaces inside the Headless Frontify DAM utilizing native GraphQL strings
- **get_account_limits**: Inspect deep internal arrays mitigating specific Picture constraints
- **get_project_assets**: Retrieve explicit Cloud logging tracing explicit Asset Limits
- **list_native_brands**: Perform structural extraction of properties driving active Global namespaces
- **list_brand_guidelines**: Identify precise active arrays spanning rented Documentation trees
- **list_workspace_projects**: Enumerate explicitly attached structured rules exporting active Workspaces
- **list_platform_users**: Retrieve the exact structural matching verifying Identity schemas
- **invite_workspace_user**: Dispatch an automated validation check routing explicit Workspace roles
- **patch_asset_metadata**: Mutate global Web CRM boundaries substituting Attributes safely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frontify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Frontify workspace"

**🤖 AI Agent:**
> Retrieving projects... I found 3 active workspaces: 'Logo Guidelines', 'Q2 Marketing Campaign', and 'Social Media Assets'. Which one would you like to explore for assets?

---

**👤 You:**
> "Show me the brand guidelines for 'Acme Corp'"

**🤖 AI Agent:**
> Retrieving guidelines... For 'Acme Corp', I found 2 registered portals: 'Global Brand Identity' and 'Technical Design System'. I can retrieve specific UI/UX constraints or rules from either portal for you.

---

**👤 You:**
> "Invite 'designer@example.com' to project 'abc-123'"

**🤖 AI Agent:**
> Invitation sent! I've commanded Frontify to add designer@example.com to project abc-123. They will receive an email to join the workspace and access the assets immediately.


## ❓ FAQ

**Q: Can my agent search for brand assets across multiple projects in Frontify?**
Yes. You can use the 'list_workspace_projects' tool to see all project IDs, and then use 'get_project_assets' or a custom 'execute_graphql_payload' to search across your entire workspace or specific brands synchronously.

**Q: How do I update the title of a digital asset via chat?**
Use the 'patch_asset_metadata' tool. Provide the 'asset_id' and the new 'title'. The agent will trigger a GraphQL mutation to substitute the attribute securely, updating the label in your Frontify DAM immediately.

**Q: Can I invite a new team member to a project through the agent?**
Absolutely. Use the 'invite_workspace_user' mutation. Provide the email address and the target Project ID. Your agent will command the backend to map the new user limit directly into the designated workspace flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frontify](https://vinkius.com/mcp/frontify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frontify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `frontify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frontify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frontify": {
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
