# LegiScan Legislation Lookup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legiscan-legislation-lookup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal legislative intelligence — search bills, votes, and state laws via AI.

## Description
Equip your AI agent with real-time legislative intelligence through the **LegiScan** MCP server. This integration provides instant access to the legislative processes of all 50 US states and Congress. Your agent can search for bills by keyword or ID, retrieve detailed bill summaries and progress, and explore voting records. Whether you are tracking specific policy changes, auditing legislative activity, or researching state laws, your agent acts as a dedicated policy analyst through natural conversation.

### What you can do

- **Bill Search** — Find legislative bills across any state or federal jurisdiction by keyword.
- **Status Tracking** — Monitor the current progress and history of specific legislation.
- **Vote Auditing** — Retrieve detailed voting records for specific bills to see how representatives voted.
- **Master List Retrieval** — Access a complete list of all active bills for a specific session and state.

### How it works

1. Subscribe to this server
2. Enter your LegiScan API Key (get it at legiscan.com)
3. Start monitoring legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Analysts & Lobbyists** — track bills and policy shifts across multiple states.
- **Legal Researchers** — access the full history and text of state-level legislation.
- **Journalists** — pull reliable legislative data for political reporting.
- **Active Citizens** — monitor the activity of their state representatives.


## Available Tools (3)
- **get_bill_details**: Get details for a specific bill
- **get_state_master_list**: Get the current master list for a state
- **search_bills**: Search for legislative bills


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LegiScan Legislation Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for California bills related to 'clean energy'."

**🤖 AI Agent:**
> Searching the LegiScan database for California... I've found several active bills related to clean energy, including AB-525 regarding offshore wind and SB-100 updates. Would you like to see the current status of a specific bill?

---

**👤 You:**
> "What is the progress of bill 'NY-S01234'?"

**🤖 AI Agent:**
> Retrieving details for NY-S01234... This bill has passed the Senate and is currently in the Assembly committee. The last action was a favorable report on June 5th. Would you like to see the voting records?

---

**👤 You:**
> "List all federal bills related to 'artificial intelligence'."

**🤖 AI Agent:**
> I've scanned the federal legislative database. There are currently 12 active bills related to AI, including the 'AI Disclosure Act' and the 'Algorithmic Accountability Act'. I can provide summaries for each of them.


## ❓ FAQ

**Q: Can I search for bills in a specific state?**
Yes! Use the `get_bill_list` tool and provide the state code (e.g., 'CA' for California, 'NY' for New York). It will return all active bills for the current session.

**Q: Does this include the full text of the bills?**
The integration currently retrieves bill summaries and status updates. For the full legal text, the tool provides reference links to the official state or federal repositories.

**Q: How can I see how my representative voted?**
Use the `get_bill_details` tool with the Bill ID. The response includes a roll call section with the results of all votes taken on that specific piece of legislation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legiscan-legislation-lookup](https://vinkius.com/mcp/legiscan-legislation-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LegiScan Legislation Lookup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legiscan-legislation-lookup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LegiScan Legislation Lookup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legiscan-legislation-lookup": {
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
