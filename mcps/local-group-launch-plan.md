# Local Group Launch Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-group-launch-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic planning engine that transforms group concepts into actionable operational frameworks.

## Description
This MCP server provides a complete suite of tools to move a local group from concept to operation. It handles the creation of a `get_launch_timeline` to map out milestones, a `get_founding_agenda` to structure the first meeting, an `get_outreach_suite` for recruiting members via opt-in messaging, and a `get_operating_plan` to manage the first quarter of activity including budget and cadence.


## Available Tools (4)
- **get_operating_plan**: Produces a structured roadmap for the first three months of operation
- **get_outreach_suite**: Provides the communication templates to recruit members
- **get_founding_agenda**: Creates the meeting structure for the very first gathering
- **get_launch_timeline**: Generates a chronological roadmap for establishing the group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Group Launch Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a launch for a local book club starting on 2025-03-01 with Alice, Bob, and Charlie."

**🤖 AI Agent:**
> The launch timeline for your book club is set. You will complete outreach by week 1, confirm members by week 2, and hold your first meeting on March 1st.

---

**👤 You:**
> "Create an agenda for our first community garden meeting. Our rules are: consensus-based decisions and monthly meetings."

**🤖 AI Agent:**
> Your founding agenda includes: 1. Introduction to the garden purpose, 2. Review of consensus-based decision rules, 3. Discussion on monthly meeting logistics.

---

**👤 You:**
> "Generate outreach messages for a hiking group to invite Dave and Eve."

**🤖 AI Agent:**
> Subject: Join our new hiking group! Hi Dave, we are forming a local hiking group and would love for you to join if you are interested.


## ❓ FAQ

**Q: What can this tool help me build?**
It helps you build a complete operational roadmap for any local group, including timelines, meeting agendas, and recruitment messages.

**Q: How does the membership model work?**
The server uses an opt-in membership model, ensuring all participants provide explicit consent before being counted toward minimum attendance requirements.

**Q: Can I manage my budget through this tool?**
Yes, the `get_operating_plan` tool allows you to input a budget and generates a structured allocation for your first three months of operation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-group-launch-plan](https://vinkius.com/en/ai-agent-connect/local-group-launch-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Group Launch Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-group-launch-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Group Launch Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-group-launch-plan": {
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
