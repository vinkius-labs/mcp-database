# Prevailing Wage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prevailing-wage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Lookup Davis-Bacon Act compliant wage rates and fringe benefits for construction trades.

## Description
The Prevailing Wage Calculator provides precise hourly base rates and fringe benefit values for various construction trades. By using tools like `lookup_prevailing_wage`, you can ensure compliance with the Davis-Bacon Act on federal and state projects by retrieving accurate labor cost data based on specific occupation, state, and county parameters.


## Available Tools (3)
- **get_supported_locations**: Get the list of supported states and counties
- **list_available_trades**: List all available construction trades
- **lookup_prevailing_wage**: g., carpenter), state (e.g., CA), and county (e.g., Los Angeles) to find hourly rates.

Lookup the prevailing wage for a specific trade and location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prevailing Wage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the prevailing wage for a carpenter in Los Angeles, CA?"

**🤖 AI Agent:**
> $45.50 per hour with $12.00 in fringe benefits.

---

**👤 You:**
> "List all available construction trades."

**🤖 AI Agent:**
> The supported trades are: carpenter, electrician, plumber, laborer, and ironworker.

---

**👤 You:**
> "Are there any supported locations in California?"

**🤖 AI Agent:**
> Yes, supported counties in California include Los Angeles, San Francisco, and San Diego.


## ❓ FAQ

**Q: How do I find the wage for a specific job?**
Use the `lookup_prevailing_wage` tool by providing the occupation, state, and county.

**Q: What trades are supported?**
You can see all supported occupations by using the `list_available_trades` tool.

**Q: How can I check which locations are covered?**
Run the `get_supported_locations` tool to see a mapping of supported states and counties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prevailing-wage-calculator](https://vinkius.com/mcp/prevailing-wage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prevailing Wage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prevailing-wage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prevailing Wage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prevailing-wage-calculator": {
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
