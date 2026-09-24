# Family Activity Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-activity-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track, categorize, and analyze family bonding through completed activities.

## Description
This MCP server provides tools to quantify family bonding time. Use `record_activity_completion` to log successful activities, `get_activity_frequency` to see how often specific categories are performed, `get_family_engagement_metrics` to evaluate bonding health, and `find_neglected_activities` to identify interests that need more attention.


## Available Tools (4)
- **find_neglected_activities**: Identify activities or categories that have not been performed recently
- **get_activity_frequency**: Determine how often certain types of activities are being performed
- **get_family_engagement_metrics**: Evaluate the health of family bonding based on participation patterns
- **record_activity_completion**: Ensure participants is a JSON array of strings.

Log a single successful instance of a family activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Activity Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record that the Smith family completed a hiking trip today."

**🤖 AI Agent:**
> Activity recorded successfully. Record ID: rec_12345, Status: completed.

---

**👤 You:**
> "How often has the Smith family done physical activities in the last 30 days?"

**🤖 AI Agent:**
> In the last 30 days, the Smith family completed 5 physical activities.

---

**👤 You:**
> "What activities has the Smith family neglected in the last 14 days?"

**🤖 AI Agent:**
> The following activities have been neglected: Reading, Board Games.


## ❓ FAQ

**Q: How do I record a new activity?**
Use the `record_activity_completion` tool with the activity ID, family ID, a list of participants, and the completion timestamp.

**Q: Can I see which activities my family is neglecting?**
Yes, the `find_neglected_activities` tool identifies activities or categories that haven't been completed within your specified threshold of days.

**Q: How is family engagement measured?**
The `get_family_engagement_metrics` tool calculates an engagement score based on participation density and activity frequency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-activity-tracker](https://vinkius.com/en/ai-agent-connect/family-activity-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Activity Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-activity-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Activity Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-activity-tracker": {
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
