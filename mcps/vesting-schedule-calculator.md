# Vesting Schedule Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vesting-schedule-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate precise monthly equity vesting timelines, identify cliff milestones, and project liquidity values.

## Description
This MCP server provides a specialized engine for managing equity compensation data. Use `generate_monthly_vesting_timeline` to create an exhaustive month-by-month breakdown of your vesting journey, identifying exactly when shares become available. The `get_cliff_milestone_details` tool allows you to extract critical cliff dates and the initial number of shares unlocked at the end of the lockout period. Additionally, use `project_liquidity_value` to estimate the potential cash value of your vested holdings during a hypothetical liquidity event like an IPO or acquisition.


## Available Tools (3)
- **generate_monthly_vesting_timeline**: Generates a month-by-month breakdown of the vesting journey
- **get_cliff_milestone_details**: Extracts critical cliff data
- **project_liquidity_value**: Estimates potential cash value of vested holdings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vesting Schedule Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a monthly vesting timeline for 1000 shares starting on Jan 1, 2024, with a 48-month period and a 12-month cliff."

**🤖 AI Agent:**
> The timeline shows zero shares released from January 2024 until January 2025. On the cliff date in January 2025, 250 shares will be released, followed by approximately 20.83 shares every month thereafter.

---

**👤 You:**
> "What is the value of 500 vested shares if the expected share price is $50?"

**🤖 AI Agent:**
> The estimated cash value for 500 shares at a price of $50 per share is $25,000.

---

**👤 You:**
> "When will my first vesting event occur if I started on March 15, 2023, with a 12-month cliff?"

**🤖 AI Agent:**
> Your first vesting event (the cliff) will occur on March 15, 2024.


## ❓ FAQ

**Q: How does the monthly timeline calculation work?**
The `generate_monthly_vesting_timeline` tool calculates a month-by-month breakdown. During the cliff period, no shares are released. On the exact date the cliff ends, a lump sum is released, followed by equal monthly increments until the end of the vesting period.

**Q: Can I estimate the value of my shares at an IPO?**
Yes, you can use the `project_liquidity_value` tool. By providing the number of shares and an expected share price, the tool calculates the estimated cash value for that event.

**Q: What information is needed to find my cliff date?**
To use `get_cliff_milestone_details`, you need your start date, the duration of the cliff period in months, and the total number of shares granted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vesting-schedule-calculator](https://vinkius.com/mcp/vesting-schedule-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vesting Schedule Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vesting-schedule-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vesting Schedule Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vesting-schedule-calculator": {
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
