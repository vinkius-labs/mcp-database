# Estimate Scope Reconciliation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/estimate-scope-reconciliation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Detect discrepancies between project baselines and revised estimates to generate approval checklists.

## Description
This MCP server provides precision tools for construction and engineering project managers to mitigate budget and schedule risks. It identifies scope changes by comparing initial baselines against revised estimates. Use `analyze_scope_drift` to detect deltas in work descriptions and costs, `reconcile_parts_discrepancies` to find missing or extra components, `evaluate_cost_impact` to quantify financial variance, and `generate_approval_checklist` to create structured verification questions for stakeholders.


## Available Tools (4)
- **analyze_scope_drift**: Detects the specific delta between an original baseline and a new revision
- **evaluate_cost_impact**: Quantifies the financial consequences of the proposed changes
- **generate_approval_checklist**: Creates a set of targeted questions for stakeholders based on the identified changes
- **reconcile_parts_discrepancies**: Identifies missing or extra physical components between two versions of a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Estimate Scope Reconciliation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two project estimates for scope drift."

**🤖 AI Agent:**
> The analysis detected a cost increase in the foundation work and two new parts added to the revised estimate.

---

**👤 You:**
> "Calculate the cost impact of a 15% budget increase."

**🤖 AI Agent:**
> The total variance is $15,000, representing a 15% increase, which is classified as Medium severity.

---

**👤 You:**
> "Check for discrepancies in the parts list."

**🤖 AI Agent:**
> The reconciliation found 2 missing parts from the baseline and 1 part with a quantity increase.


## ❓ FAQ

**Q: How does the tool detect scope changes?**
The `analyze_scope_drift` tool compares the original work descriptions and costs against the revised versions to flag additions, removals, or increased complexity.

**Q: Can I use this to find missing materials?**
Yes, the `reconcile_parts_discrepancies` tool specifically identifies missing, added, or quantity-varied parts between two project versions.

**Q: What is the purpose of the approval checklist?**
The `generate_approval_checklist` tool creates targeted questions for decision-makers to ensure they acknowledge cost and schedule impacts before approving changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/estimate-scope-reconciliation](https://vinkius.com/en/ai-agent-connect/estimate-scope-reconciliation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Estimate Scope Reconciliation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `estimate-scope-reconciliation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Estimate Scope Reconciliation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "estimate-scope-reconciliation": {
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
