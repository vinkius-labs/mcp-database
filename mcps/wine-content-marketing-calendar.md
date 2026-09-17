# Wine Content Marketing Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-content-marketing-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Generate strategic content marketing calendars for wine estates by synchronizing harvest cycles and vintage releases.

## Description
This MCP server enables wine estates and distributors to build cohesive marketing schedules. It synchronizes seasonal harvest cycles, vintage timelines, and specific wine releases into a unified editorial plan. Use `get_seasonal_template` to find wine holidays, `plan_release_content` to build teaser campaigns for new vintages, `calculate_harvest_strategy` to manage content density during picking season, and `generate_editorial_calendar` to aggregate all elements into a single distribution schedule.


## Available Tools (4)
- **generate_editorial_calendar**: Aggregates all inputs into a cohesive, unified marketing calendar
- **get_seasonal_template**: Provides a baseline set of recurring seasonal events and wine appreciation days to seed the calendar
- **plan_release_content**: Generates a high-intensity content schedule centered around a specific wine release
- **calculate_harvest_strategy**: Determines the optimal content frequency and theme distribution during the harvest window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Content Marketing Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a teaser campaign for our 2021 Cabernet Sauvignon releasing on October 15th, starting 14 days in advance."

**🤖 AI Agent:**
> Your teaser campaign for the 2021 Cabernet Sauvignon will run from October 1st to October 14th, with increasing content intensity leading up to the release on October 15th.

---

**👤 You:**
> "What seasonal wine events are happening in Napa?"

**🤖 AI Agent:**
> In the Napa region, upcoming events include the Napa Valley Harvest Festival and National Wine Day.

---

**👤 You:**
> "Generate a full marketing calendar for my estate including a harvest window from Sept 1 to Sept 30."

**🤖 AI Agent:**
> I have generated a unified marketing calendar that integrates your harvest window from September 1st to September 30th with your scheduled wine releases and seasonal events.


## ❓ FAQ

**Q: How can I plan a teaser campaign for a new vintage?**
You can use the `plan_release_content` tool. Provide the release date, the name of the wine, and how many days of lead time you want for the teaser campaign.

**Q: Can I include local wine festivals in my calendar?**
Yes. Use `get_seasonal_template` to retrieve a list of recurring seasonal events and wine appreciation days to seed your calendar.

**Q: How does the tool handle the harvest season?**
The `calculate_harvest_strategy` tool determines the optimal content frequency and theme distribution specifically for the harvest window, ensuring high-engagement storytelling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-content-marketing-calendar](https://vinkius.com/en/ai-agent-connect/wine-content-marketing-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Content Marketing Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-content-marketing-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Content Marketing Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-content-marketing-calendar": {
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
