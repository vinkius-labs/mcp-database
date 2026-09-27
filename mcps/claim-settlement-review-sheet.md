# Claim Settlement Review Sheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/claim-settlement-review-sheet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Reconcile insurance settlement statements against inventories and policy limits.

## Description
This MCP server provides precision auditing tools for insurance claims. It allows AI agents to reconcile settlement statements against itemized inventories, policy constraints, and correspondence. Use `analyze_settlement_integrity` to detect mathematical errors, `verify_item_coverage` to find missing or extra items, and `validate_policy_compliance` to ensure category limits are respected. Finally, use `generate_handler_inquiries` to produce professional questions for claims handlers based on identified discrepancies.


## Available Tools (4)
- **analyze_settlement_integrity**: Performs the core reconciliation to identify if the settlement math and coverage align with the provided policy and inventory
- **generate_handler_inquiries**: Transforms the identified discrepancies and missing information into professional, structured questions for the claims handler
- **validate_policy_compliance**: Specifically audits the settlement against the maximum financial boundaries set by the insurance policy
- **verify_item_coverage**: Checks if every high-value or specific item listed in the inventory has a corresponding entry in the settlement statement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claim Settlement Review Sheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this settlement statement matches the inventory and policy limits."

**🤖 AI Agent:**
> The settlement contains a valuation mismatch for Item #12 and exceeds the personal property limit by $500.

---

**👤 You:**
> "Are there any items from the inventory missing in the settlement?"

**🤖 AI Agent:**
> The 'High-End Camera' and 'Professional Tripod' listed in the inventory are missing from the settlement statement.

---

**👤 You:**
> "Generate questions for the claims handler regarding the identified limit breach."

**🤖 AI Agent:**
> Please provide justification for the valuation of the electronics category, as the current total exceeds the policy limit of $5,000.


## ❓ FAQ

**Q: How does the tool identify discrepancies?**
The `analyze_settlement_integrity` tool compares the settlement math, item values, and policy limits to flag mismatches.

**Q: Can I check if specific items were missed in a settlement?**
Yes, the `verify_item_coverage` tool specifically identifies items present in the inventory but missing from the settlement statement.

**Q: Does this tool help in communicating with claims handlers?**
Yes, `generate_handler_inquiries` converts all identified discrepancies into structured, professional questions for the handler.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/claim-settlement-review-sheet](https://vinkius.com/en/ai-agent-connect/claim-settlement-review-sheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claim Settlement Review Sheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claim-settlement-review-sheet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claim Settlement Review Sheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claim-settlement-review-sheet": {
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
