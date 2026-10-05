# Client Retainer Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/client-retainer-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze retainer profitability, scope drift, and payment reliability.

## Description
This MCP server provides deep analytical insights into client retainer agreements. It allows AI agents to identify profitability leaks, monitor scope creep, and assess financial risk. Use `compare_retainer_economics` to check profitability against baselines, `evaluate_scope_drift` to detect unbilled work, `analyze_payment_performance` to monitor payment delays, and `generate_client_comparison_report` to benchmark clients against the entire portfolio.


## Available Tools (4)
- **generate_client_comparison_report**: Answers how a specific client compares to the rest of the portfolio across all key metrics
- **analyze_payment_performance**: Answers how reliably a client pays their retainer fees
- **compare_retainer_economics**: Answers how profitable a specific retainer is compared to others or a baseline
- **evaluate_scope_drift**: Answers whether a client is consuming more work than they are paying for


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Client Retainer Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How profitable is retainer R-992 compared to our company baseline?"

**🤖 AI Agent:**
> Retainer R-992 has an effective hourly rate of $150, which is 15% above the company baseline profitability score.

---

**👤 You:**
> "Is client C-401 exceeding their scope of work?"

**🤖 AI Agent:**
> Yes, client C-401 has accumulated 12 hours of overage this month, indicating a scope drift trend.

---

**👤 You:**
> "Show me a comparison report for client C-101."

**🤖 AI Agent:**
> Client C-101 ranks in the top 10% of the portfolio for profitability and maintains a stable payment reliability rating.


## ❓ FAQ

**Q: How do I check if a retainer is profitable?**
You can use the `compare_retainer_economics` tool to calculate the effective hourly rate and profitability score for any specific retainer.

**Q: Can I detect if a client is exceeding their agreed scope?**
Yes, the `evaluate_scope_drift` tool identifies overage hours and the estimated value of work performed outside the defined scope.

**Q: How can I assess client payment risk?**
Use `analyze_payment_performance` to view average payment delays and reliability ratings for a specific client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/client-retainer-comparator](https://vinkius.com/en/ai-agent-connect/client-retainer-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Client Retainer Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `client-retainer-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Client Retainer Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "client-retainer-comparator": {
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
