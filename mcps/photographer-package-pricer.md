# Photographer Package Pricer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photographer-package-pricer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate professional photography quotes including labor, gear, travel, and margins.

## Description
This MCP server provides a complete pricing engine for professional photographers. It allows AI agents to calculate precise commercial quotes by aggregating shoot duration, post-production labor, logistical expenses, and professional overhead. Using tools like `get_base_rates` to find regional pricing, `calculate_operational_costs` for direct expenses, and `generate_package_quote` for final client totals, it ensures every quote accounts for equipment fees, assistant labor, and profit margins. It also includes `validate_shoot_feasibility` to ensure requested workloads stay within business capacity.


## Available Tools (4)
- **calculate_operational_costs**: Calculates the sum of all direct expenses required to perform a specific shoot
- **generate_package_quote**: Produces the final commercial quote including profit margins and taxes
- **get_base_rates**: Retrieves the standard hourly and flat rates used for calculating photography services
- **validate_shoot_feasibility**: Checks if a requested shoot configuration is possible within standard business constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photographer Package Pricer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the base rates for a Tier 2 professional in the New York region?"

**🤖 AI Agent:**
> For a Tier 2 professional in New York, the hourly shoot rate is $150, the hourly editing rate is $75, and the equipment daily rate is $200.

---

**👤 You:**
> "Calculate a quote for a 5-hour shoot with 3 hours of editing, $50 travel, $100 assistant fee, and $150 equipment fee. Use a 20% margin and 8% tax."

**🤖 AI Agent:**
> The total package price for this shoot is $1,350.00.

---

**👤 You:**
> "Is a shoot with 10 hours of shooting and 10 hours of editing feasible?"

**🤖 AI Agent:**
> No, the request is not feasible because the total labor hours exceed the maximum daily capacity.


## ❓ FAQ

**Q: How does the tool calculate the final price?**
The final price is calculated by taking the operational costs, adding the specified profit margin, and then applying the local tax percentage to that subtotal.

**Q: Can I check if a shoot is too long for my team?**
Yes, you can use `validate_shoot_feasibility` to check if the combined shoot and editing hours exceed standard daily capacity limits.

**Q: Does this include equipment costs?**
Yes, the `calculate_operational_costs` tool includes a field for equipment fees to cover gear depreciation and usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photographer-package-pricer](https://vinkius.com/en/ai-agent-connect/photographer-package-pricer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photographer Package Pricer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photographer-package-pricer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photographer Package Pricer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photographer-package-pricer": {
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
