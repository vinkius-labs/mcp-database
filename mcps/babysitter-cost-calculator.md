# Babysitter Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/babysitter-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate babysitter compensation including overtime, complexity, and travel.

## Description
This MCP server provides tools to accurately calculate babysitter compensation. It handles base rates, overtime thresholds, and service complexity multipliers. Use `get_base_cost` for initial estimates, `get_adjusted_cost` to factor in overtime or complexity, and `get_total_with_extras` to include travel stipends and minimum booking guarantees. It also includes `validate_session_parameters` to ensure rates and child counts meet service standards.


## Available Tools (4)
- **get_adjusted_cost**: Calculates the total cost including overtime and service complexity multipliers
- **get_base_cost**: Calculates the standard cost of a session before any multipliers or extra fees are applied
- **get_total_with_extras**: Provides the final amount owed to the sitter, including travel and minimum booking guarantees
- **validate_session_parameters**: Checks if a requested session configuration is valid according to standard service rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Babysitter Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the base cost for a 4 hour session at $25 per hour?"

**🤖 AI Agent:**
> The base cost for a 4 hour session at $25 per hour is $100.

---

**👤 You:**
> "Calculate the total for a 6 hour session at $20/hr with a complexity multiplier of 1.2 and a $15 travel stipend."

**🤖 AI Agent:**
> The total cost is $159, which includes the adjusted cost of $144 and a $15 travel stipend.

---

**👤 You:**
> "Is a session with 0 children valid?"

**🤖 AI Agent:**
> No, the session is invalid because the number of children must be at least one.


## ❓ FAQ

**Q: How does the tool handle overtime?**
You can use `get_adjusted_cost` to specify an `overtimeThreshold`. Any hours worked beyond this threshold are billed at a premium rate.

**Q: Can I include travel costs?**
Yes, use `get_total_with_extras` and provide a `travelStipend` value to add a fixed amount for transportation.

**Q: What happens if the total is below the minimum booking amount?**
When using `get_total_with_extras`, if the calculated sum is lower than the `minimumBookingAmount`, the tool will return the minimum amount instead.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/babysitter-cost-calculator](https://vinkius.com/en/ai-agent-connect/babysitter-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Babysitter Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `babysitter-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Babysitter Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "babysitter-cost-calculator": {
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
