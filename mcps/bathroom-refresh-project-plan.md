# Bathroom Refresh Project Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bathroom-refresh-project-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

A specialized coordination engine that transforms bathroom renovation inputs into actionable procurement, contractor, and household logistics.

## Description
This MCP server acts as a coordination hub for bathroom renovations. It manages complex renovation dependencies, calculates lead times for fixture procurement, and generates technical briefs for contractors. It also provides critical household workaround plans to manage utility loss during disruptive tasks and identifies key milestone approvals to ensure quality control throughout the project lifecycle. Use `generate_procurement_schedule` to time your purchases, `create_contractor_handoff_brief` for technical specs, `plan_household_workaround` to manage living conditions, and `get_milestone_approvals` to track project stages.


## Available Tools (4)
- **get_milestone_approvals**: Identifies key project milestones where user inspection and approval are required
- **plan_household_workaround**: Creates a plan to manage household living conditions during bathroom renovations
- **create_contractor_handoff_brief**: Generates a technical brief for contractors based on room measurements and fixture selections
- **generate_procurement_schedule**: Calculates purchase dates for fixtures to ensure they arrive on time for the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bathroom Refresh Project Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to finish my bathroom renovation by June 1st. I need a vanity (4 week lead time) and a new toilet (2 week lead time). The vanity must be installed during the finishing phase."

**🤖 AI Agent:**
> To meet your June 1st target, you should purchase the vanity by May 4th and the toilet by May 18th.

---

**👤 You:**
> "My bathroom is 5x8 feet with an 8ft ceiling. I want to replace the tub with a walk-in shower and install a modern pedestal sink."

**🤖 AI Agent:**
> Technical Brief Generated: Scope includes tub-to-shower conversion and pedestal sink installation. Room dimensions: 5' x 8' x 8'. Fixture specs: Pedestal sink (dimensions to be provided).

---

**👤 You:**
> "I am renovating my only bathroom. I need to remove the toilet and the shower. How will this affect my daily routine?"

**🤖 AI Agent:**
> Critical Disruption Warning: Removing the toilet and shower will create a zero-utility state. It is recommended to use a guest bathroom or nearby facility during these specific task windows.


## ❓ FAQ

**Q: How do I ensure my fixtures arrive before the contractor starts?**
Use the `generate_procurement_schedule` tool. By providing your fixture lead times and target completion date, it calculates exactly when you need to purchase each item to prevent downtime.

**Q: What happens if I only have one bathroom in my house?**
The `plan_household_workaround` tool is designed for this. It identifies critical disruption periods and suggests mitigation strategies to help you manage living conditions when the bathroom is unusable.

**Q: Can I use this to prepare documents for my plumber or tiler?**
Yes. The `create_contractor_handoff_brief` tool generates a technical document containing room measurements and fixture specifications, ensuring your contractors have the exact details they need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bathroom-refresh-project-plan](https://vinkius.com/en/ai-agent-connect/bathroom-refresh-project-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bathroom Refresh Project Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bathroom-refresh-project-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bathroom Refresh Project Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bathroom-refresh-project-plan": {
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
