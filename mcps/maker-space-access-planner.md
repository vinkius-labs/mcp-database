# Maker-Space Access Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/maker-space-access-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Evaluates user eligibility for maker-space access based on membership, training, and project constraints.

## Description
This MCP server acts as an intelligent decision-support engine for maker-space facilities. It evaluates whether a user is authorized to join a space by checking the intersection of their membership tier, verified safety training, and specific project requirements. Use `evaluate_access_eligibility` to determine if a user can join, `validate_tool_requirements` to check equipment compatibility, `generate_reservation_queries` to clarify booking logistics, and `create_visit_handoff` to prepare users for their first physical visit.


## Available Tools (4)
- **evaluate_access_eligibility**: Determine if a user can join a specific maker-space for their intended project
- **generate_reservation_queries**: Identify specific logistical questions to secure a booking
- **validate_tool_requirements**: Check if requested tools are compatible with user certification and facility offerings
- **create_visit_handoff**: Provide a logistical roadmap for the user's first physical visit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maker-Space Access Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I join the local Maker Hub to build a wooden birdhouse using the laser cutter?"

**🤖 AI Agent:**
> To join, you must first upgrade to a Pro membership and complete the Laser Cutter Safety Module.

---

**👤 You:**
> "I have Pro membership and Laser Cutter training. Can I use the laser cutter for my project?"

**🤖 AI Agent:**
> Yes, you are authorized to use the laser cutter for your project.

---

**👤 You:**
> "What questions should I ask to book a slot for a 4-hour session?"

**🤖 AI Agent:**
> You should ask if the 4-hour duration fits within the standard booking windows and if specific equipment reservations are required for that time block.


## ❓ FAQ

**Q: How do I know if I am allowed to use a specific tool?**
You can use `validate_tool_requirements` to compare your completed training against the tools you wish to use and what the facility provides.

**Q: What happens if my membership tier is too low?**
The `evaluate_access_eligibility` tool will return a DECLINE decision if your membership tier does not meet the minimum requirements set by the provider.

**Q: Can this tool help me prepare for my first visit?**
Yes, `create_visit_handoff` provides a logistical roadmap including arrival procedures and check-in instructions for your first visit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/maker-space-access-planner](https://vinkius.com/en/ai-agent-connect/maker-space-access-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maker-Space Access Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maker-space-access-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maker-Space Access Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maker-space-access-planner": {
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
