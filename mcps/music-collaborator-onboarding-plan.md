# Music Collaborator Onboarding Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/music-collaborator-onboarding-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [workflow-automation](../categories/workflow-automation.md)

Generate structured onboarding packets and operational workflows for musical collaborators.

## Description
This MCP server automates the onboarding process for musical projects. It provides tools to generate comprehensive onboarding packets, design first-session agendas, plan material sharing based on access levels, and define governance protocols. Use `onboarding_packet_tool` to create welcome packages, `first_session_agenda_tool` to align on meeting structures, `material_sharing_tool` to manage file transfers, and `governance_review_tool` to establish decision rights and review schedules.


## Available Tools (4)
- **first_session_agenda_tool**: 
- **governance_review_tool**: 
- **material_sharing_tool**: 
- **onboarding_packet_tool**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Music Collaborator Onboarding Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an onboarding packet for a new Mixing Engineer joining a jazz album project with Full Access."

**🤖 AI Agent:**
> The onboarding packet has been generated. It includes the project objectives for the jazz album, the specific responsibilities of the Mixing Engineer, and confirms Full Access to all project stems and session files.

---

**👤 You:**
> "Create an agenda for a first meeting with a Lyricist using Slack for communication."

**🤖 AI Agent:**
> The first session agenda is ready. It includes time for discussing creative decision rights, establishing the communication flow via Slack, and setting initial project milestones.

---

**👤 You:**
> "Plan material sharing for a Session Musician with Limited Access to existing stems."

**🤖 AI Agent:**
> The sharing plan is complete. It identifies the specific stems available for the Session Musician and lists the restricted project files that cannot be shared due to the Limited Access level.


## ❓ FAQ

**Q: How do I create a welcome package for a new producer?**
You can use the `onboarding_packet_tool` by providing the project goal, the collaborator's role, their access level, and your expectations.

**Q: Can I manage file sharing permissions?**
Yes, the `material_sharing_tool` allows you to plan file transfers while strictly respecting the defined access levels and attribution policies.

**Q: How are decision rights established?**
Decision rights and governance protocols are defined using the `governance_review_tool`, which also helps set review schedules for mutual-fit checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/music-collaborator-onboarding-plan](https://vinkius.com/en/ai-agent-connect/music-collaborator-onboarding-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Music Collaborator Onboarding Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `music-collaborator-onboarding-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Music Collaborator Onboarding Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "music-collaborator-onboarding-plan": {
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
