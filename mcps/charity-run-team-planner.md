# Charity Run Team Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/charity-run-team-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate registrations, fundraising, apparel, and travel for charity running teams.

## Description
This MCP server provides a coordination engine for managing charity run logistics. It allows AI agents to track participant registration status using `get_participant_status`, monitor collective fundraising progress with `track_fundraising_totals`, and manage apparel needs via `manage_apparel_inventory`. Additionally, teams can organize their preparation using `view_training_schedule` and `coordinate_travel_plan` to ensure all runners are ready for the event.


## Available Tools (5)
- **get_participant_status**: Get the current registration and fundraising status of a specific participant
- **manage_apparel_inventory**: Manage and view the apparel inventory requirements for a team
- **track_fundraising_totals**: Track the total fundraising progress for an entire team
- **view_training_schedule**: View the upcoming training schedule for a team
- **coordinate_travel_plan**: Coordinate and view the travel arrangements for a team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Charity Run Team Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the status of participant runner-123?"

**🤖 AI Agent:**
> Runner-123 is currently Registered, has raised $150 towards their $200 target, and is assigned a size Medium shirt.

---

**👤 You:**
> "How much has team-alpha raised so far?"

**🤖 AI Agent:**
> Team-alpha has raised $4,500 out of a total goal of $5,000, reaching 90% completion.

---

**👤 You:**
> "When is the next training session for team-beta?"

**🤖 AI Agent:**
> The next training session for team-beta is scheduled for 2024-06-15 at Central Park, requiring an intermediate skill level.


## ❓ FAQ

**Q: How can I check if a runner has met their fundraising goal?**
You can use the `get_participant_status` tool to see the `fundraisingProgress` and `targetAmount` for any specific participant.

**Q: How do I know how many shirts to order for my team?**
Use the `manage_apparel_inventory` tool to get a detailed `sizeBreakdown` of all registered participants.

**Q: Can I see the total amount raised by the whole group?**
Yes, the `track_fundraising_totals` tool provides the `totalRaised` and the `completionPercentage` for the entire team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/charity-run-team-planner](https://vinkius.com/en/ai-agent-connect/charity-run-team-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Charity Run Team Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `charity-run-team-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Charity Run Team Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "charity-run-team-planner": {
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
