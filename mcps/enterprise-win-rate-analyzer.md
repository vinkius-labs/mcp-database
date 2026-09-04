# Enterprise Win Rate Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-win-rate-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-analytics](../categories/sales-analytics.md)

Analyzes sales performance and market opportunity by segmenting enterprise deals.

## Description
This MCP server provides deep analytical insights into enterprise sales performance. It allows AI agents to decompose complex deal data into actionable metrics such as segment-specific win rates, attractiveness scores, and competitive positioning. By using tools like `get_segment_performance` and `evaluate_segment_attractiveness`, agents can identify high-value market opportunities and assess how deal complexity and buying committee size impact success. It also provides granular visibility into competitive standing via `assess_competitive_positioning` and adjusted deal health through `get_weighted_deal_metrics`.


## Available Tools (4)
- **assess_competitive_positioning**: Analyzes how the company is performing against specific competitors within each segment
- **evaluate_segment_attractiveness**: Determines which segments offer the best return on investment based on win rates and complexity
- **get_segment_performance**: Calculates the fundamental win rate and volume metrics for specific enterprise segments
- **get_weighted_deal_metrics**: Provides a granular view of deal health by adjusting for the difficulty of each deal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Win Rate Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the win rate for the 'Healthcare' and 'Finance' segments?"

**🤖 AI Agent:**
> The win rate for the Healthcare segment is 24%, and the win rate for the Finance segment is 31%.

---

**👤 You:**
> "Which segment is currently the most attractive based on current deal data?"

**🤖 AI Agent:**
> The 'Technology' segment is the most attractive, with an attractiveness score of 88 due to high win rates and manageable complexity.

---

**👤 You:**
> "How are we performing against Competitor X in the Retail segment?"

**🤖 AI Agent:**
> In the Retail segment, our market share of wins against Competitor X is 42%, with a relative win rate that is 5% higher than the segment average.


## ❓ FAQ

**Q: How does this tool calculate segment attractiveness?**
Attractiveness is calculated by balancing a segment's win rate and total deal value against the effort required, specifically accounting for deal complexity and the size of the buying committee.

**Q: Can I analyze specific competitors?**
Yes, using `assess_competitive_positioning`, you can determine your market share of wins and relative win rates against specific rivals within any given segment.

**Q: What is a weighted deal metric?**
It is an adjusted value of a deal that accounts for difficulty. The raw dollar amount is reduced based on a complexity factor to provide a more realistic view of deal health.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-win-rate-analyzer](https://vinkius.com/ai-agent-connect/enterprise-win-rate-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Win Rate Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-win-rate-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Win Rate Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-win-rate-analyzer": {
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
