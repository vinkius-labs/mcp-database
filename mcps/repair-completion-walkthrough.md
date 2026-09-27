# Repair Completion Walkthrough MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-completion-walkthrough)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Automated audit engine to validate repair work against original scopes and documents.

## Description
This MCP server acts as an automated audit engine that validates repair work against original scopes and documentation. It allows AI agents to perform line-by-line acceptance checks by comparing the Scope of Work (SOW) against observed completion items. Using tools like `analyze_scope_compliance` and `generate_punch_list`, the agent can identify missing tasks, flag discrepancies, and determine if a project is ready for final payment. It also helps protect warranty integrity by using `evaluate_warranty_claims` to ensure completed work meets specific warranty requirements.


## Available Tools (5)
- **summarize_closeout**: Provides a high-level executive summary of the entire audit
- **analyze_scope_compliance**: Compares observed completion items against the original scope to find discrepancies
- **audit_payment_readiness**: Determines if the user is financially safe to issue final payment
- **evaluate_warranty_claims**: Identifies necessary actions to protect the user's warranty rights
- **generate_punch_list**: Identifies specific deficiencies that require immediate remediation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Completion Walkthrough** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare this scope: ['Install tile', 'Paint wall'] with these observed items: ['Install tile'] and tell me what is missing."

**🤖 AI Agent:**
> The task 'Paint wall' is missing from the observed items.

---

**👤 You:**
> "The quote was $500, I have paid $400, and there is one item left on the punch list. Am I ready to pay?"

**🤖 AI Agent:**
> No, you are not ready for final payment because there is an outstanding punch list item.

---

**👤 You:**
> "Generate a punch list for these discrepancies: ['Tile color is blue instead of white', 'Paint is peeling']."

**🤖 AI Agent:**
> 1. Incorrect Tile Color (Type: incorrect, Urgency: high)
2. Peeling Paint (Type: incorrect, Urgency: medium)


## ❓ FAQ

**Q: How does the tool verify if work is complete?**
The `analyze_scope_compliance` tool compares the original scope items against the list of items actually observed to calculate a compliance rate and identify missing tasks.

**Q: Can I use this to check if I should pay my contractor?**
Yes. By using `audit_payment_readiness`, the agent checks if all punch list items are resolved and if the total amount paid aligns with the original quote.

**Q: How does it handle warranty protection?**
The `evaluate_warranty_claims` tool reviews warranty documents against the observed work to identify potential coverage risks and necessary actions like registering serial numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-completion-walkthrough](https://vinkius.com/en/ai-agent-connect/repair-completion-walkthrough)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Completion Walkthrough** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-completion-walkthrough` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Completion Walkthrough** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-completion-walkthrough": {
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
