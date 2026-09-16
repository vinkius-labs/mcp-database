# Venture Legal Fee Coverage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-legal-fee-coverage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates equitable legal fee allocation between investors and companies during venture financing rounds.

## Description
This MCP server provides specialized negotiation intelligence for venture capital transactions. It helps parties determine fair legal fee distribution by analyzing deal size, complexity, and market standards. Use `calculate_recommended_coverage` to find the ideal investor contribution, `get_cost_sharing_breakdown` to see the split between company and investor, `analyze_negotiation_range` to identify safe negotiation zones, and `evaluate_deal_scaling_impact` to adjust for economies of scale and complexity.


## Available Tools (4)
- **analyze_negotiation_range**: Identifies the safe zone for negotiators to prevent deal friction
- **calculate_recommended_coverage**: Determines the most equitable amount the investor should contribute toward legal fees
- **evaluate_deal_scaling_impact**: Adjusts fee expectations based on the volume and intricacy of the transaction
- **get_cost_sharing_breakdown**: Provides a detailed split of how the total legal expenditure should be distributed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Legal Fee Coverage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recommended investor contribution for a $5M Series A deal with $50k investor fees, $30k company fees, and a 20% cap?"

**🤖 AI Agent:**
> The recommended investor contribution is $16,000, with the company responsible for $34,000.

---

**👤 You:**
> "Show me the cost sharing breakdown for a seed round with $20,000 in total fees."

**🤖 AI Agent:**
> For a seed round, the company share is $18,000 and the investor share is $2,000, resulting in a 90/10 ratio.

---

**👤 You:**
> "What is the negotiation range for a deal where investor fees are $40,000 and company fees are $40,000 with a 25% cap?"

**🤖 AI Agent:**
> The minimum investor contribution is $20,000 and the maximum is $20,000, resulting in a high tension level.


## ❓ FAQ

**Q: How does this tool help in a Series A negotiation?**
It uses `get_cost_sharing_breakdown` with the 'series_a' tier to provide the standard split between the company and the investor based on current market practices.

**Q: Can I account for highly complex international deals?**
Yes, you can use `calculate_recommended_coverage` and set the `isHighComplexity` parameter to true to adjust the recommended contribution for multi-jurisdictional or complex structures.

**Q: How is the negotiation tension level determined?**
The `analyze_negotiation_range` tool calculates tension by comparing the requested cap against standard market practice floors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-legal-fee-coverage](https://vinkius.com/en/ai-agent-connect/venture-legal-fee-coverage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Legal Fee Coverage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-legal-fee-coverage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Legal Fee Coverage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-legal-fee-coverage": {
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
