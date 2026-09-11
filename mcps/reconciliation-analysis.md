# Reconciliation Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reconciliation-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze mine production discrepancies by comparing resource models, mine output, and mill feed.

## Description
This MCP server provides tools to perform mine reconciliation analysis. It connects AI agents to geological and production data to identify discrepancies in the mining value chain. Use `get_reconciliation_factors` to compare stages, `calculate_model_accuracy` to evaluate resource models, `calculate_adjustment_factors` for predictive corrections, and `identify_discrepancy_sources` to diagnose ore loss or dilution.


## Available Tools (4)
- **calculate_model_accuracy**: Evaluates the reliability of the geological resource model against actual production data
- **get_reconciliation_factors**: Compares different stages of the production chain to calculate specific reconciliation ratios
- **identify_discrepancy_sources**: Diagnoses whether discrepancies are caused by geological estimation errors, mining dilution, or mill recovery issues
- **calculate_adjustment_factors**: Generates correction coefficients to improve future model predictions based on historical reconciliation results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reconciliation Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reconciliation factor between the model and the mine."

**🤖 AI Agent:**
> The reconciliation factor between the model and the mine is 0.92, indicating a 8% discrepancy.

---

**👤 You:**
> "How accurate is the resource model for the current production data?"

**🤖 AI Agent:**
> The model accuracy score is 0.95, which is considered High accuracy.

---

**👤 You:**
> "What is causing the discrepancy between the model, mine, and mill?"

**🤖 AI Agent:**
> The primary source of discrepancy is Mining Dilution, with an estimated dilution percentage of 5.2%.


## ❓ FAQ

**Q: How can I compare the resource model to mine production?**
You can use the `get_reconciliation_factors` tool to compare the model stage with the mine stage.

**Q: What does the accuracy score represent?**
The accuracy score from `calculate_model_accuracy` indicates how closely the geological model's predictions align with actual mine production.

**Q: Can I identify the cause of ore loss?**
Yes, use `identify_discrepancy_sources` to diagnose if issues stem from geological estimation, mining dilution, or mill recovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reconciliation-analysis](https://vinkius.com/en/ai-agent-connect/reconciliation-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reconciliation Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reconciliation-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reconciliation Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reconciliation-analysis": {
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
