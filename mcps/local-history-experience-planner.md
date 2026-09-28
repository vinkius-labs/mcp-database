# Local History Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-history-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform historical site data into structured itineraries, preparation tasks, and engagement guides.

## Description
This MCP server acts as a specialized planning engine for historical exploration. It processes site data, user interests, and accessibility needs to generate optimized visit sequences using `plan_itinerary`. Beyond scheduling, it identifies essential preparation tasks via `generate_preparation_actions`, creates personalized engagement guides with `create_engagement_guide`, and suggests post-visit learning paths through `suggest_followup_plan`.


## Available Tools (4)
- **generate_preparation_actions**: Identifies specific tasks the user must complete to ensure a smooth visit
- **create_engagement_guide**: Provides personalized prompts for interaction and observation during the visit
- **plan_itinerary**: Generates the optimal chronological sequence of historical sites
- **suggest_followup_plan**: Offers a way to extend the learning experience after the physical tour


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local History Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 3-hour visit to the following sites: [{"name": "Old Fort", "hours": "09:00-17:00"}] with an interest in military history."

**🤖 AI Agent:**
> Your 3-hour itinerary focuses on the Old Fort. You will arrive at 09:00 for a 2-hour tour of the fortifications, followed by 1 hour of exploring the military museum exhibits.

---

**👤 You:**
> "What should I prepare for a visit to the Museum of Antiquities if I need wheelchair access?"

**🤖 AI Agent:**
> You should book the wheelchair-accessible guided tour in advance and verify the specific entrance location for the museum's ramp access.

---

**👤 You:**
> "I am interested in architecture. What should I look for at the Cathedral?"

**🤖 AI Agent:**
> Observe the intricate flying buttresses and the detailed stone carvings on the main facade to understand the Gothic structural techniques.


## ❓ FAQ

**Q: How does the itinerary generation work?**
The `plan_itinerary` tool calculates the best sequence of sites by balancing user interests, time constraints, and accessibility requirements.

**Q: Can I get tasks to prepare for my visit?**
Yes, the `generate_preparation_actions` tool provides a list of specific tasks, such as booking accessible tours, based on your planned route.

**Q: Does it provide ways to engage with site staff?**
Yes, the `create_engagement_guide` tool generates targeted questions for staff and note-taking prompts tailored to your historical interests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-history-experience-planner](https://vinkius.com/en/ai-agent-connect/local-history-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local History Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-history-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local History Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-history-experience-planner": {
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
