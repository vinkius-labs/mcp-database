# Rental Loss Claim File MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rental-loss-claim-file)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize rental damage data into structured insurance claim dossiers and evidence checklists.

## Description
This MCP server helps users consolidate fragmented rental damage data into a structured insurance claim dossier. It provides tools to `organize_claim_file` by reconciling rental agreements, damage records, and policy terms. Users can also `generate_evidence_checklist` to identify missing photos or invoices, `validate_contact_info` to ensure claimant details are complete, and `verify_policy_compliance` to check if reported damages align with insurance coverage limits.


## Available Tools (4)
- **organize_claim_file**: Consolidates diverse inputs into a single, coherent claim summary
- **verify_policy_compliance**: Checks if the specific damage types reported are covered under the provided policy terms
- **generate_evidence_checklist**: Compares provided evidence against required documentation to identify missing items
- **validate_contact_info**: Ensures the claimant and witnesses have sufficient contact information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rental Loss Claim File** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Organize my rental claim with these details: agreement {startDate: '2023-01-01', endDate: '2023-01-10', assetValue: 5000}, damages [{id: '1', type: 'windshield', cost: 300}], photos ['p1.jpg'], invoices [{id: 'i1', cost: 300}], policy {maxCoverage: 1000, coveredTypes: ['windshield']}, and event date '2023-01-05'."

**🤖 AI Agent:**
> The claim summary is complete. The total loss amount is $300, which is fully covered under your policy, resulting in a $0 coverage gap.

---

**👤 You:**
> "Check if I have all the evidence for these damages: [{id: '1', type: 'tire', cost: 200}, {id: '2', type: 'bumper', cost: 500}] with photos ['tire_photo.jpg'] and invoices [{id: 'inv_1', cost: 200}]."

**🤖 AI Agent:**
> Missing evidence detected: The bumper damage is missing both a photo and a corresponding invoice.

---

**👤 You:**
> "Validate these contacts: [{name: 'John Doe', email: 'john@example.com'}, {name: 'Jane Smith'}]."

**🤖 AI Agent:**
> Contact validation failed. Jane Smith is missing a communication method (email or phone).


## ❓ FAQ

**Q: What does the claim organizer do?**
It uses `organize_claim_file` to merge rental agreements, damage reports, and invoices into a single coherent summary for insurance submission.

**Q: How can I check if my evidence is complete?**
You can use the `generate_evidence_checklist` tool to compare your provided photos and invoices against the reported damage records.

**Q: Can I verify if my damage is covered by my policy?**
Yes, the `verify_policy_compliance` tool checks reported damage types against your specific policy terms and limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rental-loss-claim-file](https://vinkius.com/en/ai-agent-connect/rental-loss-claim-file)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rental Loss Claim File** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rental-loss-claim-file` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rental Loss Claim File** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rental-loss-claim-file": {
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
