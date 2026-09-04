# Enterprise CAC Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-cac-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate enterprise CAC, payback periods, and sales efficiency.

## Description
This MCP server provides specialized tools for analyzing Customer Acquisition Cost (CAC) in high-touch enterprise sales environments. It allows AI agents to calculate aggregate CAC using `calculate_total_cac`, break down costs by deal tier with `get_cac_by_tier`, determine the time to recoup investment via `calculate_payback_period`, and evaluate organizational scaling with `analyze_sales_efficiency`.


## Available Tools (4)
- **calculate_payback_period**: 
- **analyze_sales_efficiency**: 
- **calculate_total_cac**: 
- **get_cac_by_tier**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise CAC Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our total CAC if we spent $50k on marketing, $30k on SDRs, $40k on AEs, $20k on SEs, and closed 10 deals?"

**🤖 AI Agent:**
> The total enterprise CAC is $14,000.

---

**👤 You:**
> "Calculate the payback period for a deal with a $120,000 annual contract value, 80% gross margin, and a CAC of $30,000."

**🤖 AI Agent:**
> The payback period is 4 months.

---

**👤 You:**
> "Analyze our sales efficiency with a total CAC of $20,000, total revenue of $200,000, and a 6-month sales cycle."

**🤖 AI Agent:**
> The CAC ratio is 0.1 and the efficiency score is High.


## ❓ FAQ

**Q: How is the total CAC calculated?**
The `calculate_total_cac` tool sums all marketing, SDR, AE, and SE costs and divides them by the total number of deals closed.

**Q: Can I see the CAC for specific deal tiers?**
Yes, use the `get_cac_by_tier` tool by providing the total costs and a JSON string representing the distribution of deals across tiers.

**Q: How do I calculate the payback period?**
The `calculate_payback_period` tool calculates this by dividing the CAC by the monthly gross profit derived from the annual contract value and gross margin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-cac-analyzer](https://vinkius.com/ai-agent-connect/enterprise-cac-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise CAC Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-cac-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise CAC Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-cac-analyzer": {
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
