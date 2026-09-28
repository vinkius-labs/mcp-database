# Local Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform lifestyle constraints into a structured annual roadmap of local experiences.

## Description
This MCP server acts as a personal planning engine that converts your interests and constraints into a coherent yearly strategy. It uses tools like `generate_annual_intentions_map` to build a chronological roadmap, `identify_seasonal_decision_points` to manage environmental shifts, `suggest_membership_and_reservation_actions` to handle logistics, and `create_quarterly_review_agendas` to facilitate reflection. It helps you balance seasonal opportunities with your personal commitment limits and participation boundaries.


## Available Tools (4)
- **generate_annual_intentions_map**: Creates a high-level chronological roadmap of intended local engagement for the year
- **identify_seasonal_decision_points**: Determines when the user needs to reassess their plans due to changing seasons or environmental shifts
- **suggest_membership_and_reservation_actions**: Identifies necessary logistical steps to prepare for intended experiences based on existing access
- **create_quarterly_review_agendas**: Generates a structured guide for the user to reflect on their progress and adjust for the next quarter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a yearly plan for someone who loves nature and culinary experiences, with a high focus on outdoor activities, but cannot do more than 4 activities per month."

**🤖 AI Agent:**
> Your annual theme is 'Seasonal Exploration'. Your monthly focus will rotate between nature-based activities in spring/summer and culinary explorations in autumn/winter, staying within your 4-activity limit.

---

**👤 You:**
> "I have a museum pass and want to plan my year. What should I do?"

**🤖 AI Agent:**
> Based on your museum pass, I recommend scheduling cultural visits during the quieter winter months and setting a reservation deadline for the upcoming summer exhibition.

---

**👤 You:**
> "Help me reflect on my progress this quarter."

**🤖 AI Agent:**
> To review your progress, consider: Did you meet your primary category goals? Did you respect your participation boundaries? How well did you manage your commitment limits?


## ❓ FAQ

**Q: How does the tool handle my personal limits?**
The engine uses your `commitmentLimits` and `participationBoundaries` to ensure the generated roadmap respects your available time and activity preferences.

**Q: Can I use my existing memberships?**
Yes, the `suggest_membership_and_reservation_actions` tool specifically prioritizes your `existingPasses` to maximize the value of what you already own.

**Q: What happens when the seasons change?**
The `identify_seasonal_decision_points` tool identifies specific moments when you should reassess your plans based on seasonal triggers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-planner](https://vinkius.com/en/ai-agent-connect/local-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-planner": {
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
