# Group Activity Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-activity-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Rank and compare group activities based on cost, travel, and accessibility.

## Description
This MCP server provides a decision-support engine for planning group outings. It allows AI agents to find available activities using `find_activities`, generate prioritized lists via `calculate_rankings`, perform head-to-head comparisons with `compare_activity_pairs`, and evaluate specific needs through `get_accessibility_score`. The engine evaluates activities against logistical constraints like group size, budget, and travel effort, applying user-defined weights to find the best fit for any group.


## Available Tools (4)
- **find_activities**: Retrieves all available activities that meet the baseline availability criteria
- **calculate_rankings**: 0). Optional constraints like maxBudget or maxDuration can be provided.

Generates a ranked list of activities based on user-defined weights and group requirements
- **compare_activity_pairs**: Provides a head-to-head comparison between two specific activities
- **get_accessibility_score**: g., ["wheelchair_access", "low_noise"]).

Evaluates how well an activity accommodates specific group needs regarding accessibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Activity Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find activities available on 2025-06-15 in London."

**🤖 AI Agent:**
> I found three activities available in London on June 15th, 2025: The British Museum, Hyde Park stroll, and the London Eye.

---

**👤 You:**
> "Rank these activities for a group of 5 people, prioritizing low cost and low travel effort."

**🤖 AI Agent:**
> Based on your preferences, the top-ranked activity is the local park, followed by the community center.

---

**👤 You:**
> "Compare the Museum and the Zoo for a group that needs wheelchair access."

**🤖 AI Agent:**
> The Museum is the better choice as it provides full wheelchair access, whereas the Zoo only meets partial requirements.


## ❓ FAQ

**Q: How are activities ranked?**
Activities are ranked by normalizing metrics like cost and travel effort, then applying the weights you provide to `calculate_rankings`.

**Q: Can I filter by budget?**
Yes, you can provide a maximum budget constraint when calling `calculate_rankings` to exclude expensive options.

**Q: How does accessibility work?**
You can use `get_accessibility_score` to check how well an activity meets specific requirements like wheelchair access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-activity-comparator](https://vinkius.com/en/ai-agent-connect/group-activity-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Activity Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-activity-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Activity Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-activity-comparator": {
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
