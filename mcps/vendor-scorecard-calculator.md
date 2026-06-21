# Vendor Scorecard Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vendor-scorecard-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Calculate and monitor supplier performance using weighted metrics.

## Description
The Vendor Scorecard Calculator is a specialized MCP server designed to evaluate supplier health through multi-metric weighted scoring. By connecting your AI agent to this tool, you can process complex vendor data including OTIF, Quality, Flexibility, Cost, and Responsiveness. Use `evaluate_supplier_scores` to compute aggregate scores, `generate_performance_ranking` to sort vendors by excellence, and `detect_at_risk_vendors` to identify partners approaching critical performance thresholds.


## Available Tools
- **evaluate_supplier_scores**: Calculate weighted performance scores for vendors
- **generate_performance_ranking**: Rank vendors by their performance scores
- **detect_at_risk_vendors**: Identify vendors at risk of falling into a lower performance tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vendor Scorecard Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the scores for vendors A and B with weights: otif=40, quality=30, flexibility=10, cost=10, responsiveness=10."

**🤖 AI Agent:**
> Vendor A has a calculated score of 85.0 and Vendor B has a calculated score of 72.0.

---

**👤 You:**
> "Rank my current list of evaluated vendors from highest to lowest performance."

**🤖 AI Agent:**
> The ranked list is: 1. Vendor A (92), 2. Vendor C (85), 3. Vendor B (78).

---

**👤 You:**
> "Are any of my suppliers at risk of falling into a lower tier if their score drops by 2%?"

**🤖 AI Agent:**
> Yes, Vendor B is currently at risk as their score is near the threshold for the Conditional tier.


## ❓ FAQ

**Q: How are vendor scores calculated?**
Scores are calculated by multiplying each performance metric (like OTIF or Quality) by its assigned weight and summing the results. All weights must total 100%.

**Q: Can I identify vendors at risk of disqualification?**
Yes, by using the `detect_at_risk_vendors` tool, you can identify suppliers whose scores are approaching a lower performance tier based on a specified margin.

**Q: What metrics are supported?**
The system supports OTIF, Quality, Flexibility, Cost, and Responsiveness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vendor-scorecard-calculator](https://vinkius.com/mcp/vendor-scorecard-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vendor Scorecard Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vendor-scorecard-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vendor Scorecard Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vendor-scorecard-calculator": {
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
