# Childcare Handoff Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/childcare-handoff-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Secure and structured handoff tools for childcare transitions.

## Description
This MCP server provides a suite of tools to manage secure transitions of care between parents, caregivers, and childcare providers. It ensures safety through `generate_pickup_checklist` to verify authorized adults, and maintains continuity using `generate_handoff_brief` and `generate_followup_prompts` based on specific routine preferences. It also produces high-utility contact information via `generate_contact_card` to ensure communication permissions are strictly followed.


## Available Tools (4)
- **generate_followup_prompts**: Generates end-of-day questions for the caregiver
- **generate_contact_card**: Produces a concise contact and permission card
- **generate_handoff_brief**: Provides a structured summary of the child's status and requirements
- **generate_pickup_checklist**: Creates a verification list for pickup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Childcare Handoff Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a pickup checklist for a child with these supplies: diaper, wipes, and a change of clothes. The authorized adults are Alice and Bob."

**🤖 AI Agent:**
> Items: diaper, wipes, change of clothes. Authorized People: Alice, Bob.

---

**👤 You:**
> "Create a handoff brief for a child who naps at 1 PM and needs a bottle at 3 PM, following daycare rules that require all bottles to be labeled."

**🤖 AI Agent:**
> The child follows a schedule with a nap at 1 PM and a bottle at 3 PM. Per daycare rules, please ensure all bottles are clearly labeled.

---

**👤 You:**
> "Generate follow-up prompts for a child who has a scheduled nap time."

**🤖 AI Agent:**
> How was the nap today?


## ❓ FAQ

**Q: How does this tool ensure pickup security?**
The `generate_pickup_checklist` tool enforces authorized person precedence, ensuring only verified adults are identified for pickup.

**Q: Can I customize the handoff details?**
Yes, the `generate_handoff_brief` tool synthesizes specific routine preferences and daycare rules into a cohesive summary.

**Q: What information is included in the contact card?**
The `generate_contact_card` tool produces a card containing primary contacts, contact methods, and a summary of communication permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/childcare-handoff-brief](https://vinkius.com/en/ai-agent-connect/childcare-handoff-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Childcare Handoff Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `childcare-handoff-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Childcare Handoff Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "childcare-handoff-brief": {
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
