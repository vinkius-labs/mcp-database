# Enterprise Cross-Sell Success Rate Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-cross-sell-success-rate-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enterprise](../categories/enterprise.md)

Analyzes cross-sell efficiency, product affinity, and customer alignment.

## Description
This MCP server provides a specialized analytics engine for evaluating cross-selling effectiveness. It allows AI agents to calculate cross-sell success rates, perform product affinity analysis to find high-performing product pairs, and evaluate customer-product fit. Using tools like `calculate_success_metrics`, `analyze_product_affinity`, `evaluate_customer_fit`, and `generate_cross_sell_playbook`, sales teams can derive actionable strategic recommendations to optimize conversion metrics and product combinations.


## Available Tools (4)
- **calculate_success_metrics**: Calculates the current cross-sell efficiency metrics
- **analyze_product_affinity**: Analyzes the strength of relationships between product pairs
- **generate_cross_sell_playbook**: Generates actionable strategic recommendations for sales teams
- **evaluate_customer_fit**: Evaluates how well a product matches a customer's needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Cross-Sell Success Rate Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current cross-sell success rate if we had 100 opportunities and 25 closed sales?"

**🤖 AI Agent:**
> The current cross-sell success rate is 25% with a volume of 100 opportunities.

---

**👤 You:**
> "Which products have the strongest affinity based on these combinations: [{'productA': 'Cloud Storage', 'productB': 'Security Suite', 'conversionCount': 50}, {'productA': 'Email Pro', 'productB': 'Calendar Sync', 'conversionCount': 10}]?"

**🤖 AI Agent:**
> The strongest pair is Cloud Storage and Security Suite.

---

**👤 You:**
> "Does this product match the customer? Needs: ['Scalability', 'Low Cost'], Capabilities: ['Auto-scaling', 'Budget Tier'], Fit Score: 85"

**🤖 AI Agent:**
> The alignment score is 85, and the recommendation is to Proceed.


## ❓ FAQ

**Q: How do I calculate my current cross-sell efficiency?**
You can use the `calculate_success_metrics` tool by providing the total number of opportunities and the number of closed sales.

**Q: Can this tool help identify which products to bundle?**
Yes, the `analyze_product_affinity` tool identifies product combinations with high historical correlation to suggest effective bundles.

**Q: How does the engine provide sales recommendations?**
The `generate_cross_sell_playbook` tool synthesizes success rates, affinity data, and fit scores into a prioritized list of tactical instructions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-cross-sell-success-rate-engine](https://vinkius.com/ai-agent-connect/enterprise-cross-sell-success-rate-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Cross-Sell Success Rate Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-cross-sell-success-rate-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Cross-Sell Success Rate Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-cross-sell-success-rate-engine": {
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
