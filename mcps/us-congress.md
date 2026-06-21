# U.S. Congress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-congress)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query U.S. legislative data via AI — search bills, members, amendments, treaties, nominations, committees, and congressional records.

## Description
Connect the **U.S. Congress API** to your AI agent and access comprehensive legislative data through natural conversation.

### What you can do

- **Bill Research** — Search and browse bills across congressional sessions with full text and status tracking
- **Member Lookup** — List current and past members of Congress with biographical and voting data
- **Amendment Tracking** — Browse amendments to bills and resolutions
- **Treaty Analysis** — Access treaty submissions and their current status
- **Nomination Tracking** — Monitor presidential nominations through the confirmation process
- **Committee Navigation** — Browse congressional committees and their jurisdictions
- **Congress History** — Access session data across historical congresses

### How it works

1. Subscribe to this server
2. Get a free API key from [Congress.gov](https://api.congress.gov/sign-up/)
3. Start researching legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Researchers** — quickly find bills, track their progress, and analyze legislative trends
- **Journalists** — research congressional activity, member records, and committee hearings
- **Civic Tech Developers** — build apps that make legislative data accessible to citizens


## Available Tools
- **get_bill_details**: Get full details for a specific legislative bill
- **list_congress_amendments**: List legislative amendments
- **list_congress_bills**: gov database.

List bills from the current or specified Congress
- **list_congress_committees**: List congressional committees
- **list_congress_sessions**: g., 118th, 117th) and their start and end dates.

List historical congressional sessions
- **list_congress_members**: List current or past members of the US Congress
- **list_congress_nominations**: List executive and judicial nominations
- **list_congress_treaties**: List treaties handled by Congress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Congress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What bills about artificial intelligence were introduced in the current Congress?"

**🤖 AI Agent:**
> Found 12 bills mentioning 'artificial intelligence' in the 118th Congress. Notable: H.R.6580 'AI Accountability Act' (referred to committee), S.3312 'Responsible AI Act' (passed Senate committee). Want details on any specific bill?


## ❓ FAQ

**Q: Is the API key free?**
Yes! The Congress.gov API key is completely free. Register at api.congress.gov/sign-up/ to get instant access to all legislative data endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-congress](https://vinkius.com/mcp/us-congress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Congress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-congress` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Congress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-congress": {
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
