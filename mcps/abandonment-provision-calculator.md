# Abandonment Provision Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/abandonment-provision-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate decommissioning liabilities and annual funding requirements for offshore energy assets.

## Description
This MCP server provides specialized financial modeling tools for offshore energy decommissioning. It allows AI agents to determine the total abandonment liability using `calculate_total_liability`, calculate the necessary yearly capital allocations via `calculate_annual_provision`, and determine the current lump sum required through `calculate_present_value`. It also provides access to industry-standard cost multipliers via `get_facility_cost_benchmarks` to ensure accurate modeling of fixed platforms, FPSOs, and subsea assets.


## Available Tools (4)
- **calculate_present_value**: Calculates the current lump sum required to fund the future abandonment obligation
- **calculate_total_liability**: Determines the total estimated cost to abandon the assets at the end of their lifecycle
- **get_facility_cost_benchmarks**: Retrieves standard baseline cost multipliers and base costs for different facility types
- **calculate_annual_provision**: Calculates the yearly amount of money that must be set aside to meet the total liability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Abandonment Provision Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total abandonment liability for 10 wells on a fixed platform in 500 meters of water?"

**🤖 AI Agent:**
> The total estimated abandonment liability for 10 wells on a fixed platform at a depth of 500 meters is $150,000,000.

---

**👤 You:**
> "How much should I set aside annually for a $50M liability over 20 years with 3% inflation and 5% discount rate?"

**🤖 AI Agent:**
> The required annual contribution is $1,850,000.

---

**👤 You:**
> "What is the present value of a $100M obligation due in 15 years with a 4% discount rate?"

**🤖 AI Agent:**
> The present value of the $100,000,000 obligation is $55,526,450.


## ❓ FAQ

**Q: How do I calculate the total cost of decommissioning?**
You can use the `calculate_total_liability` tool by providing the well count, the facility type, and the water depth.

**Q: Can I account for inflation in my calculations?**
Yes, the `calculate_annual_provision` tool allows you to input an expected inflation rate to ensure your annual contributions cover future cost increases.

**Q: What is the difference between total liability and present value?**
Total liability is the estimated future cost, while `calculate_present_value` tells you how much money you need to set aside today to meet that future obligation based on a discount rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/abandonment-provision-calculator](https://vinkius.com/en/ai-agent-connect/abandonment-provision-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Abandonment Provision Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `abandonment-provision-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Abandonment Provision Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abandonment-provision-calculator": {
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
