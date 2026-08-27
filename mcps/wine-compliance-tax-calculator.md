# Wine Compliance & Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-compliance-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate federal and state wine excise taxes and manage compliance schedules.

## Description
This MCP server provides essential tools for wine producers to manage taxation and regulatory requirements. Use `calculate_federal_tax` to determine TTB obligations, `calculate_state_tax` for destination state duties, and `get_tax_in_transit_eligibility` to avoid double taxation. It also includes `generate_compliance_calendar` to track all necessary filing deadlines.


## Available Tools (4)
- **generate_compliance_calendar**: Creates a schedule of required filings and tax deadlines
- **calculate_federal_tax**: Determines the total federal excise tax owed to the TTB
- **calculate_state_tax**: Determines the excise tax owed to a specific state
- **get_tax_in_transit_eligibility**: Checks if a shipment qualifies for tax credits to avoid double taxation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Compliance & Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my federal tax for 5000 gallons if I am a small producer?"

**🤖 AI Agent:**
> Your total federal excise tax for 5,000 gallons as a small producer is $125.00.

---

**👤 You:**
> "Calculate the state tax for 1000 gallons in CA with 13% alcohol content."

**🤖 AI Agent:**
> The estimated state tax for 1,000 gallons in CA is $450.00.

---

**👤 You:**
> "Am I eligible for tax-in-transit if I ship from OR to WA?"

**🤖 AI Agent:**
> Yes, your shipment is eligible for tax-in-transit status, providing an estimated credit of $75.00.


## ❓ FAQ

**Q: How do I calculate federal excise tax?**
You can use the `calculate_federal_tax` tool by providing your total production volume and indicating if you qualify as a small producer.

**Q: Can I avoid double taxation when shipping between states?**
Yes, the `get_tax_in_transit_eligibility` tool checks if your shipment qualifies for tax credits to prevent paying taxes twice.

**Q: How do I know when my next tax filing is due?**
The `generate_compliance_calendar` tool creates a schedule of all required filings and deadlines for your specific state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-compliance-tax-calculator](https://vinkius.com/ai-agent-connect/wine-compliance-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Compliance & Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-compliance-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Compliance & Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-compliance-tax-calculator": {
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
