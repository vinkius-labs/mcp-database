# HireVue MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hirevue)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Streamline your recruitment process via HireVue — manage candidates, schedule interviews, and track positions directly from any AI agent.

## Description
Connect your **HireVue** account to any AI agent to automate and manage your hiring workflows through natural conversation.

### What you can do

- **Candidate Management** — Create, retrieve, and update candidate profiles with ease using `create_candidate`, `get_candidate`, and `update_candidate` tools.
- **Interview Orchestration** — Create interview invitations, check statuses, and cancel interviews when necessary via `create_interview`, `get_interview`, and `cancel_interview`.
- **Position Insights** — List all available job positions and fetch detailed metadata for specific roles using `list_positions` and `get_position`.
- **Workflow Automation** — Integrate hiring steps directly into your AI-driven workflows without switching tabs.

### How it works

1. Subscribe to this server
2. Enter your HireVue API Key and Base URL
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — Quickly check candidate statuses and schedule interviews without leaving the chat
- **Hiring Managers** — Review position details and candidate profiles instantly to make faster decisions
- **HR Operations** — Automate the creation of candidate records and interview invitations across the organization


## Available Tools (8)
- **create_candidate**: Create a new candidate profile
- **create_interview**: Create an interview invitation
- **get_candidate**: Get candidate details
- **get_interview**: Get interview status
- **get_position**: Get position details
- **list_positions**: List all positions
- **update_candidate**: Update an existing candidate
- **cancel_interview**: Cancel an interview


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HireVue** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available job positions in HireVue."

**🤖 AI Agent:**
> I've retrieved the available positions. You have active roles such as 'Senior Developer' (ID: pos_123) and 'Sales Lead' (ID: pos_456). Would you like details on a specific one?

---

**👤 You:**
> "Create a candidate: Jane Smith, jane.smith@example.com."

**🤖 AI Agent:**
> Candidate Jane Smith has been created successfully with ID 'cand_789'. I can now help you schedule an interview for her.

---

**👤 You:**
> "Get the details for position pos_123."

**🤖 AI Agent:**
> Fetching details for 'Senior Developer' (pos_123)... This position is active and currently has 12 associated interview templates.


## ❓ FAQ

**Q: How do I check the status of a specific interview?**
Simply use the `get_interview` tool with the specific Interview ID. The agent will retrieve the current status (e.g., 'Scheduled', 'Completed'), candidate info, and relevant timestamps.

**Q: Can I update a candidate's information after creation?**
Yes. Use the `update_candidate` tool. You can modify the `firstName`, `lastName`, `email`, or `externalId` by providing the Candidate ID and the new values.

**Q: Is it possible to cancel an interview invitation via AI?**
Yes, you can cancel an invitation using the `cancel_interview` tool. Just provide the Interview ID, and the agent will process the cancellation in HireVue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hirevue](https://vinkius.com/mcp/hirevue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HireVue** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hirevue` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HireVue** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hirevue": {
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
