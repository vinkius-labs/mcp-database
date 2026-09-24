# Accessible Bathroom Routine Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-bathroom-routine-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms bathroom configurations and privacy needs into structured daily routines and safety checklists.

## Description
This MCP server helps users with mobility or sensory needs organize their daily bathroom activities. By analyzing bathroom features, privacy priorities, and available assistive items, it generates a structured routine using `get_routine_arrangement`. It also provides a `generate_readiness_checklist` to ensure all equipment is prepared, `plan_support_handoffs` to coordinate assistance with support persons, and `create_change_request_brief` to help request environmental modifications from landlords or household managers.


## Available Tools (4)
- **create_change_request_brief**: Generates a non-clinical document to request modifications for safety or accessibility
- **generate_readiness_checklist**: Creates a checklist of items and environmental states required for the routine
- **get_routine_arrangement**: Generates a structured daily sequence of bathroom activities
- **plan_support_handoffs**: Defines the specific moments when a support person is required


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Bathroom Routine Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a bathroom routine for someone with limited mobility who needs grab bars and a shower chair, preferring high privacy."

**🤖 AI Agent:**
> Your routine includes: 1. Preparation of shower chair (Support: Independent), 2. Transfer to seat (Support: Verbal), 3. Hygiene tasks (Support: Observational). Total estimated time: 25 minutes.

---

**👤 You:**
> "Generate a checklist for my routine using a raised toilet seat and a walker."

**🤖 AI Agent:**
> Items to prepare: Raised toilet seat (Ready), Walker (Ready). Environmental checks: Floor is dry and clear of obstacles (Ready).

---

**👤 You:**
> "I need to ask my landlord for a grab bar. Can you write a brief?"

**🤖 AI Agent:**
> Summary: Request for safety modification. Requested Modification: Installation of a grab bar. Justification: To improve stability and prevent falls during daily use.


## ❓ FAQ

**Q: How does the routine account for my privacy?**
The routine uses `plan_support_handoffs` to determine if support should be observational, verbal, or physical based on your specific privacy priorities.

**Q: Can I use this to request new equipment from my landlord?**
Yes, you can use `create_change_request_brief` to generate a professional, non-clinical document that focuses on safety and environmental optimization.

**Q: What if I am missing an item needed for my routine?**
The `generate_readiness_checklist` will identify any required items that are not currently in your list of available assistive items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-bathroom-routine-planner](https://vinkius.com/en/ai-agent-connect/accessible-bathroom-routine-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Bathroom Routine Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-bathroom-routine-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Bathroom Routine Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-bathroom-routine-planner": {
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
