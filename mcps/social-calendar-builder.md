# Social Calendar Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/social-calendar-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your social life by balancing availability, budget, and travel.

## Description
Social Calendar Builder is a high-precision scheduling engine designed to manage your social commitments. It helps you navigate invitations by checking your `get_availability` to find free time, using `validate_invitation` to ensure new events fit within your schedule and budget, and monitoring your `calculate_social_load` to prevent burnout. It also uses `analyze_budget_impact` to keep your social spending on track.


## Available Tools (4)
- **analyze_budget_impact**: Projects the financial status of the social calendar for a given period
- **calculate_social_load**: Quantifies the intensity of the current schedule to prevent burnout
- **get_availability**: Determines the free time available for social engagement within a specific range
- **validate_invitation**: Checks if a specific one-off event can be added to the current schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Calendar Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When am I free to go to dinner next Tuesday?"

**🤖 AI Agent:**
> You are free next Tuesday between 6:00 PM and 10:00 PM.

---

**👤 You:**
> "Can I attend a concert this Friday that costs $50 and takes 30 minutes to get to?"

**🤖 AI Agent:**
> Yes, you have enough budget and available time to attend the concert this Friday.

---

**👤 You:**
> "How busy is my schedule for the upcoming weekend?"

**🤖 AI Agent:**
> Your social load for this weekend is low, meaning you have plenty of capacity for more activities.


## ❓ FAQ

**Q: How does the tool handle travel time?**
The tool accounts for travel time and necessary recovery buffers when validating if an invitation can be added to your schedule.

**Q: Can I track my monthly social spending?**
Yes, you can use the budget analysis features to project your financial status and ensure you stay within your monthly limits.

**Q: What is social load?**
Social load is a measure of how busy your schedule is. The tool calculates this to help you avoid over-scheduling and burnout.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/social-calendar-builder](https://vinkius.com/en/ai-agent-connect/social-calendar-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Calendar Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-calendar-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Calendar Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-calendar-builder": {
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
