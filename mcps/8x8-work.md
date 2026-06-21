# 8x8 Work MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/8x8-work)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Business communication analytics — audit call records, extension performance, and ring groups via AI.

## Description
Transform your **8x8 Work** communications data into a strategic asset for your AI agent. This integration bridges the gap between raw telephony logs and actionable business insights, allowing your agent to audit call records (CDR), monitor extension performance, and analyze ring group activity through natural language. Whether you need to track call volumes across your organization or deep-dive into a specific extension's performance, your agent provides a direct, conversational window into your 8x8 telephony environment, ensuring your communication workflows are always optimized.

### What you can do

- **Call Record Auditing (CDR)** — Retrieve detailed call journey logs and metadata for all calls across your organization.
- **Extension Performance Tracking** — Get instant summaries of call volume and performance metrics for specific extensions or posts.
- **Ring Group Analytics** — Access performance data for business ring groups to ensure optimal call distribution.
- **Communication Insights** — Audit telephony trends and usage patterns on the fly using simple conversational commands.
- **Custom Log Filtering** — Query call detail records by specific date and time ranges to find exact communication data points.

### How it works

1. Subscribe to this server
2. Enter your 8x8 API Key and Client Secret
3. Start auditing your communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IT Administrators** — audit call records and extension performance across the organization without manual log extraction.
- **Telephony Managers** — monitor ring group performance and call distribution patterns through natural language.
- **Business Operations** — track communication trends and call volumes to optimize resource allocation.
- **Customer Success Managers** — verify call activity and interaction counts for specific extensions instantly.


## Available Tools (3)
- **list_call_records**: List call detail records (CDR)
- **get_extension_summary**: Get extension call summary
- **list_ring_groups**: List ring group analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **8x8 Work** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all call records from 9 AM to 12 PM today."

**🤖 AI Agent:**
> I've retrieved the call detail records for today between 9 AM and 12 PM. There were 28 calls in total. I can provide the source, destination, and duration for each.

---

**👤 You:**
> "Give me a summary for extension 105."

**🤖 AI Agent:**
> Extension 105 summary: 15 inbound calls, 12 outbound, and an average talk time of 3 minutes. The line is currently active.

---

**👤 You:**
> "Show performance metrics for all ring groups."

**🤖 AI Agent:**
> I've retrieved analytics for your ring groups. The 'Support' group has a 98% answer rate, while 'Sales' is at 85%. Would you like more details on specific group distribution?


## ❓ FAQ

**Q: How can I see all calls made yesterday?**
Use the `list_call_records` tool and specify the start and end time for yesterday. It will return all CDR metadata for that period.

**Q: Can I check the call volume for a specific extension?**
Yes. Use the `get_extension_summary` tool and provide the extension number. You'll receive a performance summary for that specific line.

**Q: Does this integration show ring group analytics?**
Yes, use the `list_ring_groups` tool to retrieve performance data and call distribution metrics for your organization's ring groups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/8x8-work](https://vinkius.com/mcp/8x8-work)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **8x8 Work** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `8x8-work` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **8x8 Work** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "8x8-work": {
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
