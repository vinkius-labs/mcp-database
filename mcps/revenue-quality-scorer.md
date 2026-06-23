# Revenue Quality Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/revenue-quality-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze revenue stability, concentration risk, and market diversification.

## Description
The Revenue Quality Scorer provides a deep analytical dive into the health of your revenue streams. By evaluating six critical dimensions--including recurring revenue ratio, customer concentration (HHI index), expansion vs new logo mix, contractual stability, geographic diversification, and product diversity--it delivers actionable scores from 0-100. Use `summarize_revenue_quality` for a high-level overview, `analyze_concentration_risk` to identify dependency on large clients, `analyze_contractual_stability` to assess contract longevity, and `analyze_market_breadth` to measure global and product spread.


## Available Tools (4)
- **summarize_revenue_quality**: Summarize revenue quality for a given fiscal year
- **analyze_market_breadth**: Analyze market breadth and diversification
- **analyze_concentration_risk**: Analyze revenue concentration risk
- **analyze_contractual_stability**: Analyze contractual revenue stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Revenue Quality Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of our revenue quality for the 2023 fiscal year."

**🤖 AI Agent:**
> For the 2023 fiscal year, your overall revenue quality score is 78 (PREMIUM). The breakdown includes a high recurring revenue ratio and strong geographic diversification, though there is moderate concentration risk in the North American region.

---

**👤 You:**
> "How much risk are we facing from our largest customers?"

**🤖 AI Agent:**
> The concentration risk analysis shows a score of 65. Your top customer represents 12% of total revenue, which is currently within the manageable range, but monitoring is advised.

---

**👤 You:**
> "Analyze our market breadth in Europe."

**🤖 AI Agent:**
> In the Europe region, your geographic score is 85 and product score is 70. Primary revenue drivers include Enterprise Software and Cloud Services.


## ❓ FAQ

**Q: What does the overall score represent?**
The overall score is a weighted average of six dimensions: recurring revenue, concentration risk, expansion mix, stability, geography, and product diversification. A higher score indicates more predictable and stable revenue.

**Q: How can I check if a specific customer is causing high risk?**
Use the `analyze_concentration_risk` tool. By setting a `minRevenueThreshold`, you can see how much revenue is tied to your largest customers and identify if the concentration level is high risk.

**Q: Can I filter analysis by region?**
Yes, the `analyze_market_breadth` tool allows you to provide a `region` parameter to focus your geographic diversification analysis on specific areas like 'Europe' or 'North America'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revenue-quality-scorer](https://vinkius.com/mcp/revenue-quality-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Revenue Quality Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `revenue-quality-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Revenue Quality Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "revenue-quality-scorer": {
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
