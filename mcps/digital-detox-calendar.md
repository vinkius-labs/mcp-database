# Digital Detox Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-detox-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Find optimal device-free windows by balancing work, family, and wellness.

## Description
The Digital Detox Calendar is an intelligent scheduling engine designed to help you reclaim time from your digital life. By analyzing your hard constraints like work obligations and family time, it identifies contiguous blocks of free time. Using `get_available_windows`, the engine finds gaps in your schedule, while `propose_detox_slots` suggests high-quality periods that align with your sleep targets and leisure preferences. You can use `validate_detox_plan` to ensure your chosen time remains conflict-free. This tool helps you prioritize wellness by placing device-free periods where they best support your recovery and relaxation.


## Available Tools (4)
- **get_available_windows**: Identifies all possible time blocks where a user is free from all hard constraints
- **get_user_wellness_profile**: Retrieves the user's sleep targets and leisure preferences to assist in planning
- **propose_detox_slots**: Suggests specific time slots that accommodate a requested detox duration
- **validate_detox_plan**: Checks if a specific proposed detox period conflicts with any newly added or updated obligations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Detox Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me a 2-hour detox window for tomorrow."

**🤖 AI Agent:**
> I found a high-quality 2-hour window tomorrow from 2:00 PM to 4:00 PM, which aligns perfectly with your preference for afternoon reading.

---

**👤 You:**
> "Is it safe to take a break from 6 PM to 7 PM tonight?"

**🤖 AI Agent:**
> No, that period conflicts with your scheduled Family Time.

---

**👤 You:**
> "What are my current wellness preferences?"

**🤖 AI Agent:**
> Your current profile includes a sleep target of 8 hours and leisure preferences for hiking and meditation in the mornings.


## ❓ FAQ

**Q: How does the engine find the best time for a detox?**
The engine uses `propose_detox_slots` to score potential windows based on how well they align with your leisure preferences and sleep requirements.

**Q: Can I verify if a specific time is free?**
Yes, you can use the `validate_detox_plan` tool to check if a proposed period conflicts with your existing work or family obligations.

**Q: What information is needed to find available time?**
To find availability, you need to provide your user ID and the specific date you are interested in using `get_available_windows`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-detox-calendar](https://vinkius.com/en/ai-agent-connect/digital-detox-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Detox Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-detox-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Detox Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-detox-calendar": {
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
