# Repair Cost Approval Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-cost-approval-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Automates repair cost authorization workflows by applying financial rules and stage-based constraints.

## Description
This MCP server provides a workflow engine to manage repair cost authorizations. It connects AI agents to your repair management logic, allowing them to determine necessary approval steps using tools like `evaluate_approval_flow` and `get_repair_status`. The engine calculates net costs by accounting for warranty contributions and checks compliance against project deadlines using `check_deadline_compliance`. It ensures all financial decisions align with your spending caps and contact authority levels via `validate_contact_authority`.


## Available Tools (4)
- **validate_contact_authority**: Verifies if a contact has permission to approve an amount
- **check_deadline_compliance**: Determines if repair costs are valid given approaching deadlines
- **evaluate_approval_flow**: Calculates the required approval sequence
- **get_repair_status**: Retrieves the current state of a repair project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Cost Approval Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status and estimated cost for repair ID R-123?"

**🤖 AI Agent:**
> Repair R-123 is currently in the Assessment stage with a total estimated cost of $1,200 and a remaining cap of $5,000.

---

**👤 You:**
> "Determine the required approvals for repair R-456 with these rules: {"thresholds": [{"limit": 500, "contactId": "mgr_1"}]}"

**🤖 AI Agent:**
> For repair R-456, the required approval is from contact mgr_1 because the net cost falls within their authorized limit.

---

**👤 You:**
> "Is repair R-789 compliant with its deadline as of 2024-12-01?"

**🤖 AI Agent:**
> Repair R-789 is currently on track with 5 days remaining until the deadline.


## ❓ FAQ

**Q: How does the net cost calculation work?**
The net cost is calculated by taking the total estimated cost and subtracting the warranty contribution.

**Q: Can I check if a repair is overdue?**
Yes, you can use the `check_deadline_compliance` tool to determine if a repair is overdue or still on track.

**Q: What happens if a cost exceeds the spending cap?**
If the net cost exceeds the spending cap, the `evaluate_approval_flow` tool will flag that an escalation is required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-cost-approval-plan](https://vinkius.com/en/ai-agent-connect/repair-cost-approval-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Cost Approval Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-cost-approval-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Cost Approval Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-cost-approval-plan": {
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
