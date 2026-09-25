# Caregiver Responsibility Agreement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/caregiver-responsibility-agreement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured caregiving agreements, backup plans, and handoff standards to prevent burnout.

## Description
This MCP server provides a complete toolset for managing caregiving responsibilities within a family or care team. It helps prevent 'diffusion of responsibility' by enforcing a single-owner-per-task rule. Use `generate_responsibility_agreement` to create formal agreements, `generate_backup_plan` to identify secondary caregivers, `generate_handoff_standards` to ensure continuity during task transfers, and `generate_review_agenda` to prepare for periodic care reviews.


## Available Tools (4)
- **generate_backup_plan**: Identifies secondary caregivers for every active task to ensure no gaps in care
- **generate_handoff_standards**: Defines the requirements for transferring tasks between caregivers to maintain continuity
- **generate_review_agenda**: Prepares a structured meeting outline to review and update the agreement
- **generate_responsibility_agreement**: Creates the formal agreement detailing task ownership, decision rights, and communication protocols


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caregiver Responsibility Agreement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a responsibility agreement for Alice, Bob, and Charlie. Alice handles medical decisions. Bob handles groceries. Charlie handles cleaning. Use WhatsApp for communication."

**🤖 AI Agent:**
> The responsibility agreement has been generated. Alice is the authority for medical decisions. Bob is the owner for groceries, and Charlie is the owner for cleaning. All communications will occur via WhatsApp.

---

**👤 You:**
> "Help me find backups for the grocery and cleaning tasks for Alice, Bob, and Charlie."

**🤖 AI Agent:**
> For groceries (Owner: Bob), Charlie is the designated backup. For cleaning (Owner: Charlie), Bob is the designated backup.

---

**👤 You:**
> "What are the handoff standards for medical and grocery tasks?"

**🤖 AI Agent:**
> Medical tasks require High-Fidelity handoffs with detailed logs. Grocery tasks require Low-Fidelity handoffs with brief status updates.


## ❓ FAQ

**Q: How does this tool prevent confusion among family members?**
It enforces a strict one-owner-per-task rule using `generate_responsibility_agreement`, ensuring everyone knows exactly who is responsible for what.

**Q: What happens if the primary caregiver is unavailable?**
You can use `generate_backup_plan` to automatically identify suitable secondary caregivers from your list of family members.

**Q: Can I use this to prepare for family meetings?**
Yes, `generate_review_agenda` creates a structured outline including task audits, decision reviews, and capacity checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/caregiver-responsibility-agreement](https://vinkius.com/en/ai-agent-connect/caregiver-responsibility-agreement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caregiver Responsibility Agreement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `caregiver-responsibility-agreement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caregiver Responsibility Agreement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caregiver-responsibility-agreement": {
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
