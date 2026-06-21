# Lemonade MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemonade)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage Lemonade insurance — generate quotes, retrieve policy details, file claims, and handle cancellations via AI.

## Description
Connect your **Lemonade** account to any AI agent to streamline your insurance management through natural conversation. This server allows you to handle the entire lifecycle of your insurance policies without leaving your workspace.

### What you can do

- **Instant Quoting** — Generate new insurance quotes for Renters, Homeowners, or Pet insurance by providing basic address and holder information.
- **Policy Management** — Retrieve comprehensive details for any active policy, including coverage limits, deductibles, and current status.
- **Claims Processing** — File new claims directly by describing incidents, setting dates, and listing affected items.
- **Coverage Control** — Cancel active policies when they are no longer needed and receive immediate feedback on refund eligibility.

### How it works

1. Subscribe to this server
2. Enter your Lemonade API Key
3. Start managing your insurance needs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Holders** — Quickly check coverage details or file a claim without navigating complex web portals.
- **Financial Advisors** — Analyze client insurance portfolios and coverage limits through automated queries.
- **Operations Teams** — Integrate insurance quoting and management into broader financial or property management workflows.


## Available Tools
- **cancel_policy**: Cancel an active policy
- **create_quote**: Generate an insurance quote
- **file_claim**: Submit an insurance claim
- **get_policy**: Retrieve policy information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemonade** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a renters insurance quote for my apartment in New York."

**🤖 AI Agent:**
> I've initiated a quote request for renters insurance. I'll need the street address and the holder's name to finalize the details. Would you like to provide those now?

---

**👤 You:**
> "What are the coverage limits for policy POL-12345?"

**🤖 AI Agent:**
> Fetching details for policy POL-12345... Your policy is active with a liability limit of $100,000 and a $500 deductible for personal property. Would you like to see the full list of coverages?

---

**👤 You:**
> "I need to file a claim for a broken window on policy POL-98765."

**🤖 AI Agent:**
> I can help with that. I'll use the `file_claim` tool for policy POL-98765. Could you tell me the date the incident occurred and an estimated value for the window repair?


## ❓ FAQ

**Q: Can I generate a quote for my pet using this server?**
Yes! Use the `create_quote` tool and specify 'pet' as the type. You will need to provide the address and holder details to receive an accurate quote.

**Q: How do I check the coverage limits of an existing policy?**
Simply provide the Policy ID to the `get_policy` tool. The agent will return the full policy details, including limits, deductibles, and status.

**Q: Is it possible to file a claim for multiple stolen items at once?**
Yes. When using the `file_claim` tool, you can provide an array of items in the 'items' field, each with its name and value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemonade](https://vinkius.com/mcp/lemonade)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemonade** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lemonade` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemonade** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemonade": {
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
