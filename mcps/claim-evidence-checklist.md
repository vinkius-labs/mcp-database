# Claim Evidence Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/claim-evidence-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates prioritized evidence checklists for insurance claims.

## Description
This MCP server automates the generation of prioritized evidence requirements for insurance claim processing. By analyzing incident facts, policy requirements, and available records, it identifies missing proof and organizes it into an actionable checklist. Use `get_required_evidence` to identify missing items, `prioritize_checklist` to order them by urgency, `validate_evidence_sufficiency` to check if a claim is ready for decision, and `generate_owner_summary` to assign tasks to specific owners.


## Available Tools (4)
- **generate_owner_summary**: Aggregates the checklist by the person or department responsible for the items
- **prioritize_checklist**: Organizes the identified evidence into a logical, actionable order
- **get_required_evidence**: Identifies what evidence is missing or needed to satisfy the policy based on the incident
- **validate_evidence_sufficiency**: Checks if the current collection of available records is enough to move a claim to a decision phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claim Evidence Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What evidence do I need for this claim?"

**🤖 AI Agent:**
> Based on the incident facts and policy, you need to collect the following: a police report, a repair estimate, and a signed claim form.

---

**👤 You:**
> "Is the claim ready for a decision?"

**🤖 AI Agent:**
> No, there are 2 high-priority items still missing: the medical report and the witness statement.

---

**👤 You:**
> "Show me the tasks for the Adjuster."

**🤖 AI Agent:**
> The Adjuster has 3 tasks: verify the repair estimate, contact the claimant, and review the police report.


## ❓ FAQ

**Q: How do I identify what evidence is missing?**
You can use the `get_required_evidence` tool by providing the incident facts, policy requirements, and any records you already have.

**Q: Can I see which person is responsible for each task?**
Yes, the `generate_owner_summary` tool aggregates the checklist by owner so you can see exactly what each person needs to resolve.

**Q: How is the priority of evidence determined?**
The `prioritize_checklist` tool sorts items based on their due date and their criticality to the claim's validity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/claim-evidence-checklist](https://vinkius.com/en/ai-agent-connect/claim-evidence-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claim Evidence Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claim-evidence-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claim Evidence Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claim-evidence-checklist": {
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
