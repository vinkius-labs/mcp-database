# Beauty Service Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beauty-service-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare beauty service costs, travel, and annual financial impact.

## Description
This MCP server provides a decision-support engine to evaluate the total economic and logistical impact of beauty services. It allows AI agents to calculate single visit costs including tips, project annual financial commitments for recurring services, and compare different providers based on price and travel distance. Use `get_service_details` to find base pricing, `calculate_single_visit_cost` for immediate expenses, `calculate_annual_commitment` for yearly budgeting, and `compare_providers` to find the most cost-effective option.


## Available Tools (4)
- **calculate_annual_commitment**: Projects the total cost of a service over a one-year period
- **calculate_single_visit_cost**: Determines the total amount of money spent during one single appointment
- **compare_providers**: Compares two different service options to identify the most cost-effective and convenient choice
- **get_service_details**: Retrieves the base pricing and service information for a specific beauty service type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Service Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will a haircut cost if the base price is $50 and I want to tip 20%?"

**🤖 AI Agent:**
> The total cost for the haircut will be $60.00.

---

**👤 You:**
> "What is the annual cost for a manicure that costs $40 every 2 weeks?"

**🤖 AI Agent:**
> The projected annual commitment for this manicure is $1,040.00.

---

**👤 You:**
> "Compare two providers: Provider A costs $100/year and is 5 miles away, Provider B costs $120/year and is 2 miles away."

**🤖 AI Agent:**
> Provider A is the cheaper option with a cost difference of $20.00, but Provider B is closer by 3 miles.


## ❓ FAQ

**Q: How does the tool calculate the total cost of a visit?**
The `calculate_single_visit_cost` tool adds the base price of the service to the tip amount, which is calculated as a percentage of the base price.

**Q: Can I compare two different salons?**
Yes, you can use `compare_providers` to identify which salon is cheaper and which involves less travel distance.

**Q: How is the annual cost estimated?**
The `calculate_annual_commitment` tool divides 52 weeks by the frequency of your appointments to estimate the total yearly spend.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beauty-service-comparator](https://vinkius.com/en/ai-agent-connect/beauty-service-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Service Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-service-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Service Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-service-comparator": {
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
