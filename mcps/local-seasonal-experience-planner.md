# Local Seasonal Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-seasonal-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Plan perfect seasonal outings by matching local offerings with your specific needs and budget.

## Description
This MCP server acts as an intelligent planning engine for seasonal activities. It uses `plan_seasonal_experience` to orchestrate the selection of events like harvest festivals or winter markets based on your interest priorities and budget. It can also `validate_offering_viability` to ensure venues meet your accessibility needs, `calculate_logistics_and_deadlines` to manage booking windows, and `find_substitute_option` if a primary choice is unavailable.


## Available Tools (4)
- **plan_seasonal_experience**: The primary orchestrator that selects the best experience based on all user inputs
- **validate_offering_viability**: Checks a single offering against a specific set of constraints
- **find_substitute_option**: Identifies a fallback experience when the primary choice is unavailable or fails a constraint
- **calculate_logistics_and_deadlines**: Generates the necessary follow-up tasks and coordination steps for the chosen experience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Seasonal Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a seasonal experience for a group of 4 adults with a budget of $200, prioritizing culinary experiences."

**🤖 AI Agent:**
> I have selected the Autumn Harvest Food Tour. It costs $180 for the group and aligns with your culinary priority. You should book by next Tuesday to secure the reservation.

---

**👤 You:**
> "Find a winter activity that is wheelchair accessible for a family of 3."

**🤖 AI Agent:**
> The Winter Lights Display is the best option. It is fully wheelchair accessible and fits your family size.

---

**👤 You:**
> "What happens if my first choice for a summer festival is too expensive?"

**🤖 AI Agent:**
> The system will automatically use `find_substitute_option` to identify a more affordable local community festival that still matches your interests.


## ❓ FAQ

**Q: How does the planner handle my budget?**
The engine respects your budget ceiling strictly. If no offerings fit within your limit, it will use `find_substitute_option` to look for alternatives that do.

**Q: Can I include accessibility requirements?**
Yes. The tool uses `validate_offering_viability` to check if a venue can accommodate specific mobility, sensory, or dietary needs.

**Q: Will I know when I need to book?**
Yes, the `calculate_logistics_and_deadlines` tool generates specific time-sensitive actions and booking deadlines for your selected experience.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-seasonal-experience-planner](https://vinkius.com/en/ai-agent-connect/local-seasonal-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Seasonal Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-seasonal-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Seasonal Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-seasonal-experience-planner": {
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
