# FCC Telecom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fcc-telecom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Search the official USA telecommunications database to audit corporate Internet Providers and Interconnected VoIP carriers.

## Description
The **FCC Telecom MCP Server** lets your AI agent search the Universal Service Administrative Company (USAC) and federal Form 499 databases. Easily audit whether a telecom company is legally registered to operate within the United States.

### Core Capabilities

- **Carrier Financial Registration** — Confirm the active legal registration numbers (FRN) assigned to any modern telecom business.
- **VoIP Auditing** — Trace Interconnected VoIP vendors and evaluate structural transparency instantly.
- **Corporate Discovery** — Type any partial corporate name and let the AI extract real registered names straight from public accountability ledgers.


## Available Tools (2)
- **lookup_filer_by_id**: Lookup a specific Telecommunications operator by their exact FCC Form 499 Filer ID
- **search_telecom_filers**: Perform a fuzzy string search across the national telecom database by company brand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FCC Telecom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find details for the telecom provider with Filer ID 829223."

**🤖 AI Agent:**
> I checked the Form 499 database. Filer 829223 corresponds to an active VoIP carrier and their corporate structure operates normally.

---

**👤 You:**
> "Can you check if ExampleCorp provides certified internet services?"

**🤖 AI Agent:**
> Let me search the registry... I found ExampleCorp. They are officially registered as a major Interconnected Telecom Carrier with a validated FRN.

---

**👤 You:**
> "List all active operational filings tied to FRN ending in 456 last year."

**🤖 AI Agent:**
> Extracting administrative filings reliably...
Scanning matching records isolated 2 major reports (Form 499-A) legally cleared systematically without discrepancies.


## ❓ FAQ

**Q: Is this data pulled from official resources?**
Yes. This taps directly directly into public Form 499 and overarching USAC/FCC open-data mandates to bring legitimate records to your workspace.

**Q: Why build an AI tool solely for Telecom registration?**
Because transparency matters. Easily confirming a company is properly registered eliminates logistical blind-spots for enterprise research workflows.

**Q: Can I query historical data and past performance?**
Yes, you can pull complete structural histories covering specific chronological windows tracking compliance across multiple filing years seamlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fcc-telecom](https://vinkius.com/mcp/fcc-telecom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FCC Telecom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fcc-telecom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FCC Telecom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fcc-telecom": {
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
