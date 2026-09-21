# Creator Revenue Split MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creator-revenue-split)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Reconcile multi-party revenue distributions and calculate exact payouts.

## Description
This MCP server manages the complex revenue waterfall for creators and their stakeholders. It provides tools to calculate exact monetary splits, simulate the impact of contract changes on net earnings, and verify the mathematical integrity of multi-tier distributions. Use `calculate_revenue_distribution` to determine party-level amounts, `analyze_creator_payout_impact` to test new contract terms, `get_tax_and_compliance_summary` to view ecosystem leakage, and `validate_split_integrity` to ensure all splits balance perfectly with the gross revenue.


## Available Tools (4)
- **analyze_creator_payout_impact**: 
- **calculate_revenue_distribution**: 
- **get_tax_and_compliance_summary**: 
- **validate_split_integrity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creator Revenue Split** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the split for $1000 gross revenue with 30% platform, 50% creator, 10% manager, and 10% tax."

**🤖 AI Agent:**
> The distribution is: Platform $300.00, Creator $500.00, Manager $100.00, and Tax $100.00.

---

**👤 You:**
> "How much will the creator lose if the manager's share increases from 10% to 15% on $5000 revenue?"

**🤖 AI Agent:**
> The creator's net earnings will decrease by $250.00.

---

**👤 You:**
> "Check if this split is valid: $100 gross, 50% creator, 50% manager."

**🤖 AI Agent:**
> The split is balanced. Creator receives $50.00 and Manager receives $50.00.


## ❓ FAQ

**Q: How does the tool handle rounding discrepancies?**
The `calculate_revenue_distribution` tool calculates a `roundingResidual` to ensure the sum of all party splits exactly matches the gross revenue.

**Q: Can I simulate a manager's commission increase?**
Yes, use `analyze_creator_payout_impact` to compare current net earnings against proposed contract changes.

**Q: What is considered 'leakage' in the compliance summary?**
Leakage is defined as the combined total of platform fees and tax obligations extracted from the gross revenue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creator-revenue-split](https://vinkius.com/en/ai-agent-connect/creator-revenue-split)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creator Revenue Split** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creator-revenue-split` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creator Revenue Split** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creator-revenue-split": {
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
