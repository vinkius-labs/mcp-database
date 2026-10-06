# Creator Campaign Rate Card MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creator-campaign-rate-card)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise creator deliverable pricing based on production, reach, and usage rights.

## Description
This MCP server provides a specialized pricing engine for influencer marketing campaigns. It allows AI agents to calculate total campaign costs by processing production labor, audience reach premiums, legal usage rights, and exclusivity restrictions. Use `calculate_base_production_cost` to establish the initial talent and labor cost, `apply_reach_premium` to adjust for audience size, `calculate_usage_and_exclusivity_fees` to add legal and competitive premiums, and `finalize_campaign_price` to apply the final agency margin.


## Available Tools (4)
- **apply_reach_premium**: Adjusts the base cost to account for the value of the creator's audience size
- **finalize_campaign_price**: Applies the final profit margin to reach the client-facing price
- **calculate_base_production_cost**: Determines the initial cost of a deliverable based solely on labor and talent
- **calculate_usage_and_exclusivity_fees**: Calculates additional costs for legal rights and competitive restrictions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creator Campaign Rate Card** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the base production cost for a creator with 10 hours of work at $150/hour and a $500 talent fee."

**🤖 AI Agent:**
> The total base cost is $2,000.

---

**👤 You:**
> "What is the final price for a subtotal of $5,000 with a 20% profit margin?"

**🤖 AI Agent:**
> The final price is $6,250.

---

**👤 You:**
> "Adjust a $1,000 base cost for an audience reach of 50,000 followers."

**🤖 AI Agent:**
> The adjusted cost after applying the reach premium is $1,500.


## ❓ FAQ

**Q: How do I calculate the initial cost of a creator?**
You should use the `calculate_base_production_cost` tool, providing the estimated production hours, the creator's hourly rate, and their flat talent fee.

**Q: Can I account for exclusivity restrictions?**
Yes, the `calculate_usage_and_exclusivity_fees` tool allows you to specify if a creator is exclusive and for how many days.

**Q: How is the final client price determined?**
The final price is determined by using `finalize_campaign_price`, which applies a specified profit margin to the accumulated subtotal of all costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creator-campaign-rate-card](https://vinkius.com/en/ai-agent-connect/creator-campaign-rate-card)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creator Campaign Rate Card** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creator-campaign-rate-card` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creator Campaign Rate Card** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creator-campaign-rate-card": {
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
