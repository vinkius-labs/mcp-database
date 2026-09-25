# Neighborhood Skill-Share Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/neighborhood-skill-share-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinates skill-sharing sessions by matching participants, venues, and materials.

## Description
This MCP server acts as a coordination engine for community skill-sharing. It processes skill offers and requests to create organized session calendars. Using `generate_session_calendar`, it matches participants based on availability and consent. It also handles host assignments via `assign_session_hosts`, generates material checklists with `create_materials_checklist`, and develops communication plans through `plan_participant_communications` while respecting user privacy.


## Available Tools (4)
- **assign_session_hosts**: Identifies and assigns a primary host for every session in the calendar
- **create_materials_checklist**: Generates a list of necessary items for each scheduled session
- **generate_session_calendar**: Creates a structured schedule of all valid skill-sharing sessions
- **plan_participant_communications**: Produces a notification plan to inform participants of their scheduled sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neighborhood Skill-Share Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a skill-sharing schedule for these participants: [{"name": "Alice", "offers": ["Gardening"], "availability": "Weekends", "consent": true}, {"name": "Bob", "requests": ["Gardening"], "availability": "Weekends", "consent": true}] and these venues: [{"name": "Community Park", "capacity": 5}]"

**🤖 AI Agent:**
> A gardening session has been scheduled for this weekend at the Community Park with Alice and Bob participating.

---

**👤 You:**
> "Generate a materials checklist for a woodworking session."

**🤖 AI Agent:**
> The required materials for the woodworking session are: hammer, nails, and sandpaper.

---

**👤 You:**
> "Assign a host for the scheduled cooking session."

**🤖 AI Agent:**
> Charlie has been assigned as the host for the cooking session.


## ❓ FAQ

**Q: How are skill matches determined?**
Matches are made using `generate_session_calendar` only when a skill offer meets a request, both parties have overlapping availability, and both have provided consent.

**Q: Can I control how I am contacted?**
Yes. The `plan_participant_communications` tool respects all participant consent preferences and contact methods.

**Q: How are hosts selected for sessions?**
The `assign_session_hosts` tool identifies participants who have explicitly consented to hosting or provided a venue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/neighborhood-skill-share-planner](https://vinkius.com/en/ai-agent-connect/neighborhood-skill-share-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neighborhood Skill-Share Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neighborhood-skill-share-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neighborhood Skill-Share Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neighborhood-skill-share-planner": {
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
