# Travel Insurance Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-insurance-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare travel insurance policies by cost, coverage, and risk scenarios.

## Description
This MCP server connects AI agents to a comprehensive travel insurance comparison engine. It allows for retrieving available policies via `get_available_policies`, comparing direct costs with `compare_policy_financials`, testing specific risks using `evaluate_risk_scenario`, and identifying coverage gaps with `check_policy_exclusions`. It is designed to help travelers find the best financial protection for their specific trip costs and planned activities.


## Available Tools (4)
- **compare_policy_financials**: Compare the direct monetary costs (premiums and deductibles) between specific policies
- **evaluate_risk_scenario**: Determine which policy provides the best financial protection for a specific hypothetical event
- **get_available_policies**: Retrieve a list of all insurance policies currently available in the system for comparison
- **check_policy_exclusions**: Identify which policies exclude coverage for specific activities or conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Insurance Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What travel insurance policies are available in the USA?"

**🤖 AI Agent:**
> The available policies in the USA are: Standard Tier (Premium: $50), Premium Tier (Premium: $120), and Elite Tier (Premium: $250).

---

**👤 You:**
> "Compare the costs for policy ID 'pol_123' and 'pol_456' for a trip costing $3000."

**🤖 AI Agent:**
> For a $3000 trip, policy 'pol_123' has a total upfront cost of $100 and $200 out-of-pocket exposure, while 'pol_456' has a total upfront cost of $150 and $50 out-of-pocket exposure.

---

**👤 You:**
> "Which policy is best for a $500 medical emergency scenario?"

**🤖 AI Agent:**
> The Elite Tier policy provides the best protection for a $500 medical emergency, offering a net recovery of $500 due to its minimal deductible.


## ❓ FAQ

**Q: How can I see which insurance policies are available?**
You can use the `get_available_policies` tool to retrieve a list of all currently available insurance products, optionally filtering by a specific region.

**Q: Can I test how a policy handles a specific event like lost luggage?**
Yes, the `evaluate_risk_scenario` tool allows you to simulate specific events like lost baggage or medical emergencies to see the net recovery for each policy.

**Q: How do I know if an activity like skydiving is covered?**
You can use `check_policy_exclusions` to identify if specific activities or conditions are excluded from coverage in the selected policies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-insurance-comparator](https://vinkius.com/en/ai-agent-connect/travel-insurance-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Insurance Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-insurance-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Insurance Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-insurance-comparator": {
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
