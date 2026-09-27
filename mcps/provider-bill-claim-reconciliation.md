# Provider Bill & Claim Reconciliation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/provider-bill-claim-reconciliation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Reconcile medical invoices against benefit schedules and EOBs to identify discrepancies.

## Description
This MCP server provides specialized tools to audit medical billing. It identifies mismatches between provider invoices, insurance benefit schedules, and Explanations of Benefits (EOB). Use `analyze_reconciliation_discrepancies` to find pricing or coverage errors, `calculate_patient_responsibility` to determine exact patient owes, `validate_claim_integrity` to ensure document consistency, and `generate_evidence_sequence` to prepare audit-ready document flows.


## Available Tools (4)
- **calculate_patient_responsibility**: Determine exactly how much a patient should owe based on the intersection of the invoice and the benefit schedule
- **analyze_reconciliation_discrepancies**: Identify all mismatches between provided medical billing documents
- **generate_evidence_sequence**: Determine the correct chronological and logical order of documents needed to resolve a discrepancy
- **validate_claim_integrity**: Verify that all submitted documents belong to the same clinical visit or service period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Provider Bill & Claim Reconciliation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify any mismatches in these billing documents."

**🤖 AI Agent:**
> The discrepancy report shows a pricing error of $50.00 on line item 'Consultation' because the invoice charge exceeds the allowed amount in the benefit schedule.

---

**👤 You:**
> "How much should the patient pay for this service?"

**🤖 AI Agent:**
> The total patient responsibility is $45.00, consisting of a $20.00 copay and a $25.00 deductible application.

---

**👤 You:**
> "What is the order of documents I need to submit for an audit?"

**🤖 AI Agent:**
> To resolve this overcharge, you should first provide the Invoice, followed by the Benefit Schedule, then the EOB, and finally the Receipt.


## ❓ FAQ

**Q: What kind of discrepancies can this tool find?**
It identifies pricing errors, coverage mismatches, payment discrepancies, and duplicate billing using `analyze_reconciliation_discrepancies`.

**Q: How do I know if my documents belong to the same claim?**
You can use the `validate_claim_integrity` tool to verify that all submitted documents share the same provider ID and service period.

**Q: Can I calculate how much a patient owes?**
Yes, the `calculate_patient_responsibility` tool determines the expected copay, deductible, and total amount owed based on the benefit schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/provider-bill-claim-reconciliation](https://vinkius.com/en/ai-agent-connect/provider-bill-claim-reconciliation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Provider Bill & Claim Reconciliation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `provider-bill-claim-reconciliation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Provider Bill & Claim Reconciliation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "provider-bill-claim-reconciliation": {
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
