# PE Deal Sourcing ROI Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pe-deal-sourcing-roi-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate PE deal sourcing ROI and optimize channel budget allocation.

## Description
This MCP server provides specialized tools for Private Equity firms to analyze the efficiency of their deal sourcing channels. It calculates critical metrics like cost per closed deal and channel ROI using the `analyze_channel_efficiency` tool. Users can determine budget priorities with `rank_sourcing_priorities`, compare the effectiveness of proprietary versus intermediary channels via `compare_proprietary_vs_intermediary`, and forecast the impact of capital shifts using `simulate_budget_reallocation`.


## Available Tools (4)
- **analyze_channel_efficiency**: Calculates the core performance metrics for individual sourcing channels
- **compare_proprietary_vs_intermediary**: Evaluates whether direct proprietary sourcing is more cost-effective than using external intermediaries
- **rank_sourcing_priorities**: Determines which channels should be prioritized for budget allocation based on ROI and cost
- **simulate_budget_reallocation**: Predicts how changes in channel spending would impact the total number of closed deals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PE Deal Sourcing ROI Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the efficiency of my sourcing channels: 'Direct Outreach' with 50 deals, 20% IC rate, and €10,000 cost, and 'Bank Referral' with 30 deals, 10% IC rate, and €25,000 cost. The average time to close is 6 months."

**🤖 AI Agent:**
> Direct Outreach has a cost per closed deal of €1,000 with a high ROI, while Bank Referral has a cost per closed deal of €8,333. Direct Outreach is the more efficient channel.

---

**👤 You:**
> "Which sourcing channels should I prioritize for my next budget cycle based on these metrics?"

**🤖 AI Agent:**
> Based on the current efficiency metrics, you should prioritize 'Direct Outreach' as it offers the lowest cost per closed deal and highest ROI.

---

**👤 You:**
> "What happens if I move €5,000 from my lowest performing channel to my highest performing one?"

**🤖 AI Agent:**
> Reallocating €5,000 is projected to increase your total closed deals by 3 and improve your overall channel ROI by 12%.


## ❓ FAQ

**Q: How do I calculate the ROI for a specific sourcing channel?**
You can use the `analyze_channel_efficiency` tool. Provide the channel data including deal flow, IC rate, and costs to receive a full efficiency profile including ROI.

**Q: Can I compare direct sourcing against investment banks?**
Yes, the `compare_proprietary_vs_intermediary` tool is designed specifically to evaluate if proprietary methods are more cost-effective than intermediaries.

**Q: How can I predict the outcome of moving budget between channels?**
Use the `simulate_budget_reallocation` tool. It takes current efficiency metrics and a budget shift amount to project changes in total closed deals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pe-deal-sourcing-roi-analyzer](https://vinkius.com/en/ai-agent-connect/pe-deal-sourcing-roi-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PE Deal Sourcing ROI Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pe-deal-sourcing-roi-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PE Deal Sourcing ROI Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pe-deal-sourcing-roi-analyzer": {
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
