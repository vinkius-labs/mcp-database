# Wedding Budget Reality Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wedding-budget-reality-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Singapore wedding budget calculator and reality check.

## Description
Plan your big day with precision using the Wedding Budget Reality Check. This tool provides a complete financial breakdown for Singaporean weddings, including base costs for romance, banquet, or elopement styles. It calculates total expenses by accounting for venue tiers, photography, attire, rings, and honeymoon. Most importantly, it estimates your angbao recovery and calculates the net out-of-pocket cost, helping you determine exactly how many months of savings you need to reach your goal. Use `calculate_wedding_estimate` for a full breakdown, `analyze_savings_plan` to test different savings rates, or `compare_wedding_types` to see how different styles impact your budget.


## Available Tools (3)
- **analyze_savings_plan**: Evaluates how monthly savings impact the time to reach a budget
- **calculate_wedding_estimate**: 
- **compare_wedding_types**: Compares financial impact of different wedding styles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Budget Reality Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a wedding estimate for a banquet with 150 guests at a hotel tier."

**🤖 AI Agent:**
> For a banquet with 150 guests at a hotel, your base cost is 45,000 SGD. Including additional costs like photography, gown, rings, and honeymoon, your total wedding cost is 75,000 SGD. With an estimated angbao recovery of 30,000 SGD, your net cost is 45,000 SGD. At a savings rate of 1,000 SGD per month, it will take 75 months to save.

---

**👤 You:**
> "How long will it take to save 15,000 SGD if I save 1,200 SGD per month?"

**🤖 AI Agent:**
> It will take 12.5 months to reach your goal of 15,000 SGD by saving 1,200 SGD per month.

---

**👤 You:**
> "Compare the costs for 50 guests at a restaurant venue."

**🤖 AI Agent:**
> For 50 guests at a restaurant: an elopement style costs 17,000 SGD net, a romance style costs 32,000 SGD net, and a banquet style costs 25,000 SGD net.


## ❓ FAQ

**Q: How is the angbao recovery calculated?**
The tool estimates angbao recovery by multiplying the expected guest count by an average gift amount of 200 SGD per guest.

**Q: Can I compare different wedding styles?**
Yes, you can use the `compare_wedding_types` tool to see the financial difference between romance, banquet, and elopement styles for a specific guest count.

**Q: What does the net cost represent?**
The net cost is the final amount you need to pay out-of-pocket after subtracting the estimated angbao recovery from the total wedding cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wedding-budget-reality-check](https://vinkius.com/ai-agent-connect/wedding-budget-reality-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Budget Reality Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-budget-reality-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Budget Reality Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-budget-reality-check": {
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
