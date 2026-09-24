# Accessible Home Entry Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-home-entry-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Plan non-prescriptive entry arrangements, decision-maker briefs, and visitor protocols for improved home access.

## Description
This MCP server provides a strategic planning framework for improving home entrance accessibility without prescribing construction work. It helps users organize their physical space, communicate needs to landlords via a `create_decision_maker_brief` tool, and manage visitor interactions through `draft_visitor_instructions`. Users can also optimize their immediate environment using `generate_entry_arrangement` and develop long-term strategies with `build_phased_action_plan`.


## Available Tools (4)
- **create_decision_maker_brief**: Creates a formal communication brief for decision-makers like landlords or building managers
- **draft_visitor_instructions**: Drafts instructions for visitors or delivery personnel to assist with entry
- **generate_entry_arrangement**: Generates a non-prescriptive entry arrangement based on physical constraints and user needs
- **build_phased_action_plan**: Builds a phased roadmap for improving entry access over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Home Entry Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me organize my entrance. The door is 32 inches wide, I usually carry heavy groceries, and I value safety and speed."

**🤖 AI Agent:**
> To optimize your 32-inch entrance for grocery delivery, we suggest placing a stable landing zone for bags immediately inside the door and ensuring the path is clear of obstacles to maintain speed and safety.

---

**👤 You:**
> "I need to ask my building manager for permission to adjust the entryway layout. The rules say no permanent changes can be made."

**🤖 AI Agent:**
> Your formal request will emphasize that the proposed adjustments are non-structural and respect all current building rules while addressing your specific accessibility needs.

---

**👤 You:**
> "Create instructions for my Amazon delivery driver. I have a steep step at the entrance and I need packages left on the porch mat."

**🤖 AI Agent:**
> Please leave all packages on the porch mat located at the base of the entrance step to ensure they are accessible and secure.


## ❓ FAQ

**Q: Does this tool recommend construction or renovations?**
No. The tool is strictly non-prescriptive. It focuses on organizational adjustments, behavioral changes, and optimizing existing space rather than suggesting structural or construction work.

**Q: How can I use this to talk to my landlord?**
You can use the `create_decision_maker_brief` tool. It generates a formal request that aligns your needs with existing building rules to minimize friction with property managers.

**Q: Can I prepare instructions for delivery drivers?**
Yes, the `draft_visitor_instructions` tool allows you to create specific guidance for different visitor types, such as couriers or medical professionals, to ensure safe and effective entry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-home-entry-planner](https://vinkius.com/en/ai-agent-connect/accessible-home-entry-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Home Entry Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-home-entry-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Home Entry Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-home-entry-planner": {
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
