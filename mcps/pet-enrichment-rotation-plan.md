# Pet Enrichment Rotation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-enrichment-rotation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Automated scheduling and logistics for pet enrichment activities and item rotation.

## Description
This MCP server provides a complete logistics engine for managing pet enrichment. It uses `get_rotation_plan` to generate rotating activity schedules, `get_household_assignments` to delegate tasks to available members, and `get_prep_and_cleanup_instructions` for operational steps. It also includes `evaluate_refresh_need` to determine when to cycle in new items based on usage history and replacement rules.


## Available Tools (4)
- **evaluate_refresh_need**: Calculates whether the current enrichment cycle should be reset or updated
- **get_household_assignments**: Determines who is responsible for specific tasks related to the enrichment plan
- **get_prep_and_cleanup_instructions**: Provides the specific operational steps for handling enrichment items
- **get_rotation_plan**: Generates the full rotating activity schedule and associated logistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Enrichment Rotation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a rotation plan for my dog using my approved items and activities."

**🤖 AI Agent:**
> Here is your rotating activity plan: Monday: Kong Toy (Puzzle), Wednesday: Snuffle Mat (Search), Friday: Fetch (Physical).

---

**👤 You:**
> "Who is responsible for cleaning up the Snuffle Mat today?"

**🤖 AI Agent:**
> Based on current availability, Sarah is assigned to the cleanup task for the Snuffle Mat activity.

---

**👤 You:**
> "Should I refresh my enrichment items this month?"

**🤖 AI Agent:**
> Yes, a refresh is recommended because the current rotation has reached its maximum age according to your rules.


## ❓ FAQ

**Q: How do I generate a new schedule?**
You can use the `get_rotation_plan` tool by providing your approved items, activities, and household availability.

**Q: Can I assign tasks to specific people?**
Yes, the `get_household_assignments` tool matches tasks like preparation and cleanup to members available during the activity window.

**Q: How does the system know when to change toys?**
The `evaluate_refresh_need` tool checks the current rotation age and item usage history against your defined replacement rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-enrichment-rotation-plan](https://vinkius.com/en/ai-agent-connect/pet-enrichment-rotation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Enrichment Rotation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-enrichment-rotation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Enrichment Rotation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-enrichment-rotation-plan": {
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
