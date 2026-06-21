# Postman MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postman-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Design, test, and document APIs collaboratively with the world most popular API development platform used by millions of developers.

## Description
Connect your **Postman** organizational account to any AI agent and take full control of your API development and documentation workflows through natural conversation.

### What you can do

- **Workspaces & Collections** — List all personal and team workspaces and fetch API collections directly from the Postman cloud
- **Request Management** — Query all recorded requests (both headers and body) from any target collection using its unique ID
- **Deep Environment Inspection** — Fetch complete variable sets, values, and precise configurations for specific environments
- **API Documentation** — List API definitions and schemas to understand and integrate with internal or external services
- **Infrastructure Monitoring** — Retrieve the status of scheduled monitors and mock servers to ensure service availability

### How it works

1. Subscribe to this server
2. Enter your Postman API Key from your account settings
3. Start managing your API resources from Claude, Cursor, or any MCP-compatible client

No more wrestling with complex UI tabs to find documentation or variable values. Your AI acts as a dedicated API architect or technical lead assistant.

### Who is this for?

- **Software Engineers** — instantly retrieve request details, check environment variables, and inspect schemas without leaving your IDE
- **QA Teams** — verify monitor statuses and test collections straight from your communication hub
- **Technical Leads** — automate organizational querying to orchestrate cross-functional API documentation smoothly


## Available Tools
- **get_collection_details**: Get details and requests for a specific collection
- **get_environment_details**: Get variables and details for an environment
- **get_workspace_details**: Get details and items for a specific workspace
- **list_apis**: APIs represent a higher-level grouping that can include multiple versions and schemas.

List all API definitions
- **list_collections**: Collections are used to group and share related API requests.

List all API collections
- **list_environments**: Environments allow for managing variables across different stages like development or production.

List all environment variable sets
- **list_mocks**: Mock servers simulate API responses before the actual API is implemented.

List all configured mock servers
- **list_monitors**: Monitors help ensure API performance and availability.

List all scheduled collection monitors
- **list_workspaces**: Workspaces are the primary organizational unit in Postman.

List all accessible Postman workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postman** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Postman workspaces."

**🤖 AI Agent:**
> I've fetched your workspaces. You currently have access to: 'Core Payments API' (ID: ws-123) and 'Partner Integrations' (ID: ws-456). Which one would you like to explore?

---

**👤 You:**
> "Show me the items in collection ID [ID]."

**🤖 AI Agent:**
> Accessing collection... I found 8 requests inside. Key endpoints include 'POST /login' and 'GET /user/profile'. Would you like the full details of the '/user/profile' request?

---

**👤 You:**
> "Check the status of my API monitors."

**🤖 AI Agent:**
> Running the check... All 3 monitors are currently active. 'Production Health' passed its last run, while 'Staging API' reported a minor latency warning. Should I drill down into the 'Staging' results?


## ❓ FAQ

**Q: Can my AI automatically find the details of a specific collection just by providing its ID?**
Yes! Use the `get_collection_details` tool with the unique ID. Your agent will respond with complete structure, requests, and metadata in seconds.

**Q: How do I check my API monitors status?**
Simply ask the agent to run the `list_monitors` tool. It will compile all scheduled monitors and their latest results configured for your environment.

**Q: Does the integration permit modifying collections?**
No. The core set of tools focuses strictly on querying and analyzing API context—listing workspaces, collections, and environments. State alteration operations are not currently exposed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postman-alternative](https://vinkius.com/mcp/postman-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postman** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `postman-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postman** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postman-alternative": {
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
