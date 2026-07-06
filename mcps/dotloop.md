# Dotloop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dotloop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage real estate transactions via Dotloop — list loops, manage participants, and oversee documents.

## Description
Connect your AI agent to **Dotloop**, the leading real estate transaction management platform. This integration allows you to interact with your loops, manage participants, and oversee documents and tasks directly through natural conversation.

### What you can do

- **Loop Oversight** — List and retrieve detailed information for all your real estate transactions
- **Participant Management** — Add, list, and update profiles for buyers, sellers, and agents involved in a loop
- **Document Organization** — Explore folders and list metadata for all transaction documents
- **Task Tracking** — Monitor the status of checklists and to-do items for each deal
- **Activity Auditing** — Review the full activity log for any specific loop to see historical actions
- **Profile Control** — Access multiple profiles (personal or brokerage) associated with your account

### How it works

1. Subscribe to this server
2. Enter your **Dotloop Access Token** (obtained from the Dotloop Developer Center)
3. Start managing your real estate deals through natural language

### Who is this for?

- **Real Estate Agents** — quickly check the status of loops and participants during a busy day
- **Transaction Coordinators** — oversee document completion and task progress across multiple deals
- **Brokerage Administrators** — audit activity and manage contacts within the brokerage profile


## Available Tools (10)
- **list_profile_contacts**: List all contacts in the user directory for a specific profile
- **list_folder_documents**: List all documents within a specific loop folder
- **list_loop_folders**: List all document folders within a specific loop
- **list_loops**: List all real estate transactions (loops) for a specific profile
- **list_loop_participants**: List all participants (buyers, sellers, agents) in a specific loop
- **list_profiles**: Retrieve all profiles (brokerages, associations, individual) associated with the user
- **list_loop_tasks**: List all tasks and checklists for a specific loop
- **add_loop_participant**: Add a new participant to a loop
- **get_loop_details**: Get comprehensive information for a specific loop
- **get_loop_activity**: Retrieve the activity log for a specific loop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dotloop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active transaction loops."

**🤖 AI Agent:**
> Fetching loops... I found several active transactions, including '123 Main St' (Under Contract) and '456 Oak Ave' (Pre-Listing). Would you like to see the participants for any of them?

---

**👤 You:**
> "Show me the tasks for loop ID '78901'."

**🤖 AI Agent:**
> Retrieving tasks for loop '78901'... I found 5 items: 3 completed (Signed Disclosure, Inspection Scheduled) and 2 pending (Review Appraisal, Final Walkthrough).


## ❓ FAQ

**Q: How do I get an API Access Token for Dotloop?**
You must register as a developer at the [**Dotloop Developer Center**](https://info.dotloop.com/developers). Once your application is approved, you can utilize OAuth 2.0 to generate an access token for your account.

**Q: Does this tool support document signing?**
This MCP server is optimized for data retrieval, oversight, and management of participants/tasks. For the actual signing process, you should continue to use the Dotloop web or mobile application.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dotloop](https://vinkius.com/mcp/dotloop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dotloop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dotloop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dotloop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dotloop": {
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
