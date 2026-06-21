# Superblocks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/superblocks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build and manage internal tools and workflows — list applications, manage configurations, and generate secure embed tokens directly from your AI agent.

## Description
Connect your **Superblocks** organization to any AI agent to streamline the management of your internal applications and automated workflows. This server allows you to orchestrate your low-code ecosystem through natural language.

### What you can do

- **Application Management** — List all organizational applications, fetch detailed configurations, and create or update apps programmatically.
- **Workflow Orchestration** — Retrieve a comprehensive list of all active workflows to monitor your backend logic and scheduled jobs.
- **Secure Embedding** — Generate authenticated session tokens for Embedded Apps, enabling seamless SSO integration for your end-users.
- **Lifecycle Control** — Perform maintenance by updating application payloads or deleting obsolete resources directly from your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Superblocks API Key
3. Start managing your internal tooling infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Internal Tools Engineers** — quickly audit application configurations and manage resource lifecycles without leaving the terminal or IDE.
- **DevOps Teams** — monitor active workflows and automate the deployment or update of Superblocks applications.
- **Product Managers** — list available internal tools and generate embed tokens for stakeholder reviews or client integrations.


## Available Tools (7)
- **create_application**: Create a new Superblocks application
- **create_embed_token**: Used to request session tokens for users when embedding Superblocks applications via SSO.

Create an authenticated session token for Embedded Apps
- **delete_application**: Delete a Superblocks application
- **get_application**: Retrieve details for a specific application
- **list_applications**: Supports pagination.

List all applications in the organization
- **list_workflows**: List all workflows in the organization
- **update_application**: Update an existing Superblocks application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Superblocks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 applications in our Superblocks organization."

**🤖 AI Agent:**
> I've retrieved the first 10 applications. You have tools like 'Customer Support Dashboard' (ID: app_123) and 'Inventory Manager' (ID: app_456) active. Would you like details on any specific one?

---

**👤 You:**
> "Show me the configuration for application ID app_789."

**🤖 AI Agent:**
> Fetching details for app_789... This is the 'Sales Analytics' app. It currently has 3 pages and connects to your Snowflake and Salesforce instances. Would you like to see the full JSON payload?

---

**👤 You:**
> "Generate an embed token for user 'dev@example.com' for our embedded portal."

**🤖 AI Agent:**
> I've generated a secure session token for dev@example.com. You can now use this token to authenticate their session in your embedded Superblocks components.


## ❓ FAQ

**Q: How can I see all the internal tools currently built in my organization?**
You can use the `list_applications` tool. It retrieves a paginated list of all Superblocks applications, allowing your AI to browse through your entire internal tool library.

**Q: Is it possible to generate a login token for a user to view an embedded app?**
Yes, the `create_embed_token` tool is designed specifically for this. Provide the user's email and optional metadata to receive a secure session token for Embedded Apps.

**Q: Can I check the status of my backend workflows and scheduled jobs?**
Absolutely. Use the `list_workflows` tool to get a full inventory of all workflows in your organization, which helps in monitoring your automated processes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/superblocks](https://vinkius.com/mcp/superblocks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Superblocks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `superblocks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Superblocks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "superblocks": {
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
