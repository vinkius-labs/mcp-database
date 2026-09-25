# Care Transition Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-transition-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Coordinate care transitions with dependency gates and consent rules.

## Description
This MCP server provides a coordination engine for managing transitions between care arrangements. It uses dependency gates to ensure prerequisites like transport are met and enforces Transfer-of-Information (TOI) consent rules for medical records. Use `get_transition_timeline` to map out the move, `generate_checklist` for packing and vital records, `create_notification_plan` to schedule stakeholder communications, and `build_support_roster` to organize the first week of support.


## Available Tools (4)
- **create_notification_plan**: Outlines who needs to be notified and when
- **generate_checklist**: Produces a comprehensive list of items to pack and documents to secure
- **get_transition_timeline**: Generates a chronological roadmap of the transition process
- **build_support_roster**: Organizes the human resources needed for the first week of the new arrangement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Transition Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a transition timeline for moving from home care to a nursing facility starting 2024-11-01 and ending 2024-11-05, where transport is not yet confirmed."

**🤖 AI Agent:**
> The transition timeline is being prepared. Note: A critical path gap exists because transport has not been confirmed.

---

**👤 You:**
> "Create a packing and records checklist for a move. Belongings: wheelchair, walker, favorite chair. Records: medical history, insurance card. Consent is not granted."

**🤖 AI Agent:**
> Packing List: wheelchair, walker, favorite chair. Records List: medical history, insurance card. WARNING: Consent not granted; certain records cannot be transferred.

---

**👤 You:**
> "Build a support roster for a new assisted living facility. Responsible people: Jane (Primary), John (Support). Transport is via specialized van."

**🤖 AI Agent:**
> The 7-day support roster has been generated, assigning Jane and John to specific monitoring tasks based on the assisted living requirements.


## ❓ FAQ

**Q: How does the tool handle medical record security?**
The `generate_checklist` tool enforces Transfer-of-Information (TOI) consent. If consent is not granted, the tool will issue warnings that certain records cannot be transferred.

**Q: Can I see the critical path for my transition?**
Yes, by using `get_transition_timeline`, the tool identifies critical path gaps if required dependencies are not satisfied.

**Q: What is included in the support roster?**
The `build_support_roster` tool generates a structured 7-day schedule of personnel and tasks to monitor the individual during their first week in the new arrangement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-transition-planner](https://vinkius.com/en/ai-agent-connect/care-transition-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Transition Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-transition-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Transition Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-transition-planner": {
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
