# Data Broker Removal Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/data-broker-removal-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize and monitor personal data deletion requests across data brokers.

## Description
This MCP server provides a centralized system for managing personal data opt-out requests. It allows users to track the status of individual requests using `track_request_status`, identify requests awaiting confirmation via `list_pending_verifications`, and flag requests requiring immediate attention with `list_overdue_followups`. Users can also monitor overall progress and success rates through `get_completion_summary`. It is designed to ensure compliance with privacy regulations by managing submission dates, verification deadlines, and follow-up intervals.


## Available Tools (4)
- **get_completion_summary**: 
- **list_overdue_followups**: 
- **list_pending_verifications**: 
- **track_request_status**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Broker Removal Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the status of request ID 12345?"

**🤖 AI Agent:**
> The request 12345 is currently in 'submitted' status with a verification deadline of 2024-12-01.

---

**👤 You:**
> "Show me all pending verifications for Acme Corp."

**🤖 AI Agent:**
> There are 2 pending requests for Acme Corp: ID 9876 (deadline 2024-11-15) and ID 5432 (deadline 2024-11-20).

---

**👤 You:**
> "Give me a summary of my removal requests."

**🤖 AI Agent:**
> You have submitted 10 requests in total. 4 have been completed, 1 was refused, and 5 are currently active.


## ❓ FAQ

**Q: How can I check the status of a specific request?**
You can use the `track_request_status` tool by providing the unique requestId for the specific opt-out request.

**Q: How do I know if a follow-up is overdue?**
Use the `list_overdue_followups` tool to identify requests where the scheduled follow-up time has passed without a resolution.

**Q: Can I filter requests by a specific broker?**
Yes, most tools like `list_pending_verifications` and `get_completion_summary` allow you to filter results by providing a brokerName.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/data-broker-removal-tracker](https://vinkius.com/en/ai-agent-connect/data-broker-removal-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Data Broker Removal Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `data-broker-removal-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Data Broker Removal Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "data-broker-removal-tracker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
