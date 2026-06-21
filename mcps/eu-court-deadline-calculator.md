# EU Court Deadline Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-court-deadline-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate legal procedural deadlines across European jurisdictions, accounting for national holidays and business day adjustments.

## Description
The EU Court Deadline Calculator is a specialized engine designed to determine legal procedural deadlines within various European jurisdictions. By providing a country code, an event type (such as response, appeal, or execution), and the date of the triggering event, the tool calculates the final deadline while automatically accounting for weekends and national holidays. It uses `calculate_deadline` to find the adjusted date, `check_holiday_status` to verify specific dates, and `list_jurisdictions` to identify supported countries. This ensures that legal professionals can accurately track deadlines without manual calendar checking.


## Available Tools
- **calculate_deadline**: Calculates the final legal deadline based on a triggering event and specific legal parameters
- **check_holiday_status**: Verifies if a specific calendar date is recognized as a public holiday in a chosen country
- **list_jurisdictions**: Provides a valid list of supported countries and court levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Court Deadline Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the deadline for a response in France for an event that happened on 2024-05-01."

**🤖 AI Agent:**
> The calculated deadline is 2024-05-15. The tool used `calculate_deadline` with countryCode: 'FR', eventType: 'response', and eventDate: '2024-05-01'.

---

**👤 You:**
> "Check if 2024-12-25 is a holiday in Germany."

**🤖 AI Agent:**
> The `check_holiday_status` tool confirms that 2024-12-25 is a recognized public holiday in Germany (DE).

---

**👤 You:**
> "List all available jurisdictions."

**🤖 AI Agent:**
> The `list_jurisdictions` tool returned the supported countries and court levels, including National and EU tiers.


## ❓ FAQ

**Q: How does the tool handle holidays?**
If a calculated deadline falls on a weekend or a registered national holiday in the specified country, the engine automatically postpones the deadline to the next available business day.

**Q: Which countries are supported?**
You can use the `list_jurisdictions` tool to see a complete list of all currently supported ISO alpha-2 country codes and court levels.

**Q: What types of legal procedures can I calculate?**
The engine supports calculating deadlines for 'response', 'appeal', and 'execution' event types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-court-deadline-calculator](https://vinkius.com/mcp/eu-court-deadline-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU Court Deadline Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eu-court-deadline-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU Court Deadline Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-court-deadline-calculator": {
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
