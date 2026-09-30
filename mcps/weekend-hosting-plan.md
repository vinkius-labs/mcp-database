# Weekend Hosting Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekend-hosting-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate guest stays with complete timelines, meal schedules, and prep checklists.

## Description
Manage every aspect of guest hosting with precision. This MCP server provides tools to generate complete itineraries using `plan_hosting_timeline`, optimize meal timings with `calculate_meal_schedule`, and manage sleeping arrangements via `allocate_sleeping_arrangements`. You can also prepare for arrivals with `generate_prep_checklist` and ensure everything is perfect by using `audit_hosting_plan` to validate your logistics.


## Available Tools (5)
- **allocate_sleeping_arrangements**: Verifies and assigns sleeping locations based on guest count and available capacity
- **audit_hosting_plan**: Validates an existing plan to ensure no constraints are violated
- **calculate_meal_schedule**: Determines the optimal timing for breakfast, lunch, and dinner
- **generate_prep_checklist**: Creates a list of necessary tasks to complete before the guest arrival
- **plan_hosting_timeline**: Generates a complete, chronologically ordered itinerary covering all hosting aspects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekend Hosting Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a hosting timeline for 4 guests arriving on Friday at 5 PM and leaving Sunday at 11 AM."

**🤖 AI Agent:**
> I have generated your hosting timeline. It includes preparation tasks before Friday 5 PM, scheduled meals for the weekend, and a post-departure reset for Sunday.

---

**👤 You:**
> "I have 3 guests and 2 king beds. Can you help me with sleeping arrangements?"

**🤖 AI Agent:**
> I have allocated the sleeping arrangements. One guest will be assigned to a king bed, and the remaining two guests will share the second king bed.

---

**👤 You:**
> "What should I do to prepare before my guests arrive on Saturday morning?"

**🤖 AI Agent:**
> Your preparation checklist includes cleaning the guest rooms, grocery shopping for the planned meals, and setting up the bedding for 3 guests.


## ❓ FAQ

**Q: How do I generate a full itinerary?**
Use the `plan_hosting_timeline` tool by providing the arrival time, departure time, and guest count.

**Q: Can I check if my plan has enough beds?**
Yes, use `allocate_sleeping_arrangements` to verify and assign sleeping locations based on your guest count and bed capacity.

**Q: How can I ensure my meal times are well-spaced?**
The `calculate_meal_schedule` tool determines optimal timing for breakfast, lunch, and dinner to avoid long gaps between meals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekend-hosting-plan](https://vinkius.com/en/ai-agent-connect/weekend-hosting-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekend Hosting Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekend-hosting-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekend Hosting Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekend-hosting-plan": {
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
