# Auto Insurance Deductible Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/auto-insurance-deductible-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare auto insurance policies by analyzing annual costs across different claim scenarios.

## Description
This MCP server provides tools to evaluate auto insurance options by calculating total annual expenditures. Use `get_insurance_options` to find available policies, `calculate_scenario_costs` to see how specific claim amounts impact your budget, and `get_policy_rankings` to find the most cost-effective coverage. You can also use `compare_premium_vs_deductible` to analyze the financial trade-offs of different deductible levels for a specific carrier.


## Available Tools (4)
- **calculate_scenario_costs**: Calculates the total annual cost for each insurance option based on specific claim scenarios
- **compare_premium_vs_deductible**: Analyzes the trade-off between different deductible levels for a single carrier
- **get_insurance_options**: Retrieves the available insurance policy configurations for comparison
- **get_policy_rankings**: Provides a stable, prioritized list of insurance options based on cost efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Auto Insurance Deductible Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the available insurance options in the USA?"

**🤖 AI Agent:**
> The available insurance options in the USA include Standard, Economy, and Premium tier policies from various carriers.

---

**👤 You:**
> "Compare the total annual cost for policy ID 'pol_123' if I have two claims of $500 and $1500."

**🤖 AI Agent:**
> For policy 'pol_123', the total annual cost with claim amounts of $500 and $1500 is $1,250.

---

**👤 You:**
> "Show me the ranking of policies for claim amounts of $1000, $2000, and $5000."

**🤖 AI Agent:**
> Based on those claim amounts, the top-ranked policy is 'SafeDrive Auto' with a total annual cost of $850, followed by 'BudgetGuard' at $920.


## ❓ FAQ

**Q: How is the policy ranking determined?**
Ranking is primarily determined by the lowest total annual cost across your provided claim scenarios. If two policies have the same cost, the one with the lower deductible is ranked higher.

**Q: Can I filter policies by geographic region?**
Yes, you can use the `get_insurance_options` tool to filter available policies by region, specifically supporting USA and Europe.

**Q: What does the risk profile indicate?**
The risk profile labels policies as 'Low Risk' if they have low deductibles or 'High Risk' if they have high deductibles, helping you understand your out-of-pocket exposure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/auto-insurance-deductible-comparator](https://vinkius.com/en/ai-agent-connect/auto-insurance-deductible-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Auto Insurance Deductible Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `auto-insurance-deductible-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Auto Insurance Deductible Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "auto-insurance-deductible-comparator": {
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
