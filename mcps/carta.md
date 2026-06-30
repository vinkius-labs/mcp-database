# Carta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/carta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to Carta — query cap tables, review equity grants, and monitor 409A valuations without opening the equity management dashboard.

## Description
Connect **Carta** to your AI agent and manage your company's equity operations, stakeholder information, and compliance data conversationally.

### What you can do

- **Cap Table Queries** — Retrieve your company's capitalization table including shares outstanding, share classes, and ownership percentages.
- **Equity Grants** — List active stock option grants, vesting schedules, exercise windows, and grant statuses.
- **409A Valuations** — Access your latest 409A valuation data and fair market values for compliance reporting.
- **Stakeholder Directory** — Query your shareholder registry to find individual equity positions and contact details.

### How it works

1. Subscribe to the Carta integration on the marketplace.
2. Create an OAuth app in the Carta Developer Portal (developer.carta.com → Create App → copy Client ID and Client Secret).
3. Ask your AI agent to query cap tables, check vesting schedules, or pull 409A data.

### Who is this for?

- **Founders & CEOs** — Get instant answers about dilution, ownership percentages, and equity pool availability during board meetings.
- **HR & People Ops** — Check vesting schedules and grant details for employees without navigating the Carta dashboard.
- **CFOs & Legal Teams** — Pull 409A valuations and compliance data instantly for audits and fundraising diligence.


## Available Tools (10)
- **list_stakeholders**: List all stakeholders
- **list_companies**: List all companies
- **list_valuations**: List 409A valuations
- **get_company**: Get company details
- **list_securities**: List all securities
- **list_share_classes**: with liquidation preferences and conversion rights.

List share classes
- **list_option_plans**: List stock option plans
- **list_funding_rounds**: List funding rounds
- **list_convertibles**: List convertible notes and SAFEs
- **get_cap_table**: Get the full cap table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our current cap table summary."

**🤖 AI Agent:**
> Your cap table shows 10,000,000 authorized shares with 7,200,000 issued. Founders hold 45%, Series A investors 25%, option pool is 20% (800,000 remaining unallocated), and employee grants account for 10%.

---

**👤 You:**
> "What's our latest 409A valuation?"

**🤖 AI Agent:**
> Your latest 409A was completed on March 15, 2025, with a fair market value of $2.85 per share (Common Stock). The valuation is valid until September 15, 2025.

---

**👤 You:**
> "How many shares has João Paulo vested so far?"

**🤖 AI Agent:**
> João Paulo was granted 50,000 options on June 1, 2023, with a 4-year vesting schedule and 1-year cliff. He has vested 21,875 shares (43.75%). His next vesting event is on the 1st of next month for 1,041 shares.


## ❓ FAQ

**Q: How do I get my Carta API credentials?**
Go to the **Carta Developer Portal** at **developer.carta.com** and log in or register. Click **Create App**, fill in the app details (name, homepage URL, grant type, and required scopes), then click **View app details** to find your **Client ID** and **Client Secret**. Copy both values and paste them into the configuration below. Note: Carta's API program is invite-only — if you don't have access, email **developers@carta.com** to request it.

**Q: Can my AI agent tell me exactly how much equity remains in our option pool?**
Yes. Ask your agent to pull the cap table and it returns the total authorized shares, shares issued, options granted, options exercised, and the remaining unallocated pool — giving you an instant snapshot of your equity position. Perfect for board meetings, fundraising conversations, or new-hire planning where you need the numbers immediately.

**Q: What if a new hire asks about their vesting schedule during onboarding?**
Your AI agent can pull any employee's grant details including total shares granted, vesting start date, cliff date, monthly vesting rate, and shares already vested — so HR can answer equity questions instantly during the onboarding call without opening the Carta dashboard or asking Legal.

**Q: Can this handle companies with complex multi-round fundraising histories?**
Yes. The integration retrieves the full cap table structure including Seed, Series A, B, C rounds and beyond, convertible notes, SAFEs, and all share classes. Perfect for late-stage startups preparing for IPO, companies running secondary sales, and legal teams performing due diligence on cap table complexity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/carta](https://vinkius.com/mcp/carta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carta": {
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
