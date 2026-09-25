# Care Volunteer Support Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-volunteer-support-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Coordinates volunteer rosters, task briefs, and safety protocols for care organizations.

## Description
This MCP server provides a coordination system that translates organizational requirements and recipient preferences into actionable volunteer rosters, task instructions, and safety-compliant check-in protocols. It uses tools like `get_volunteer_roster` to assign staff, `generate_task_briefs` to create instructions, `get_checkin_protocol` for safety verification, and `create_followup_plan` to ensure duty of care through structured communication.


## Available Tools (4)
- **create_followup_plan**: Establishes a communication schedule between volunteers and coordinators to ensure duty of care
- **get_volunteer_roster**: Generates a list of volunteers assigned to specific tasks based on schedule needs and organization requirements
- **generate_task_briefs**: Creates detailed instruction sets for volunteers that incorporate task limits and recipient needs
- **get_checkin_protocol**: Provides the specific safety and verification steps a volunteer must follow when starting a session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Volunteer Support Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a volunteer roster for Monday morning shifts with 3 volunteers needed."

**🤖 AI Agent:**
> The roster has been generated: Alice (Meal Delivery, 08:00-10:00), Bob (Check-in, 08:00-09:00), and Charlie (Errands, 09:00-11:00).

---

**👤 You:**
> "Create a task brief for a meal delivery task where the recipient prefers quiet service."

**🤖 AI Agent:**
> Task: Meal Delivery. Instructions: Deliver the meal to the front door. Recipient Note: Please keep noise to a minimum as the recipient prefers quiet service. Boundary Alert: Do not enter the residence.

---

**👤 You:**
> "What is the check-in protocol for the community center access?"

**🤖 AI Agent:**
> 1. Use the side entrance code 1234. 2. Sign the visitor log. 3. Notify Supervisor Sarah at 555-0199 upon arrival.


## ❓ FAQ

**Q: How are volunteers assigned to tasks?**
Volunteers are assigned using the `get_volunteer_roster` tool, which matches schedule needs and organization requirements against volunteer vetting status.

**Q: How does the system ensure volunteer safety?**
Safety is maintained through the `get_checkin_protocol` tool, which provides specific access rules and mandatory coordinator notifications.

**Q: Can I customize instructions for specific recipients?**
Yes, the `generate_task_briefs` tool allows you to incorporate recipient preferences and task boundaries into detailed instructions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-volunteer-support-plan](https://vinkius.com/en/ai-agent-connect/care-volunteer-support-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Volunteer Support Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-volunteer-support-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Volunteer Support Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-volunteer-support-plan": {
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
