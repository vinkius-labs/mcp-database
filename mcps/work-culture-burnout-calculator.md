# Work Culture Burnout Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/work-culture-burnout-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify burnout risk and work intensity for extreme work cultures.

## Description
This MCP server provides deterministic tools to measure the impact of extreme work patterns, such as '996' or 'Black Company' cultures. Use `generate_burnout_profile` to get a complete health overview, or specific tools like `evaluate_karoshi_risk` to assess health hazards. It calculates weekly work intensity, annual commute burden, and the Karoshi Risk Index to help identify unsustainable labor conditions.


## Available Tools (4)
- **evaluate_karoshi_risk**: Assess the level of health risk associated with the weekly workload
- **calculate_annual_commute_burden**: Calculate the total annual time lost to commuting
- **calculate_weekly_work_intensity**: Determine the total effective work hours performed in one week
- **generate_burnout_profile**: Provide a comprehensive overview of work-life health metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Work Culture Burnout Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my burnout profile: I work 10 hours a day, 6 days a week, with 20 hours of overtime per month and a 45-minute commute."

**🤖 AI Agent:**
> Your weekly work hours are 65.0, your Karoshi Risk Index is 100 (Critical), and your annual commute burden is 486 hours.

---

**👤 You:**
> "What is my Karoshi risk if I work 45 hours a week?"

**🤖 AI Agent:**
> Your Karoshi Risk Index is 50 (Warning).

---

**👤 You:**
> "How much time do I lose to commuting annually if I work 5 days a week and commute for 30 minutes each way (60 minutes total daily)?"

**🤖 AI Agent:**
> Your annual commute burden is 260 hours.


## ❓ FAQ

**Q: What is the Karoshi Risk Index?**
The Karoshi Risk Index is a metric that categorizes the risk of death from overwork. A score of 100 indicates critical risk (over 60 hours/week), 50 indicates warning (40-60 hours/week), and 0 indicates safe levels.

**Q: How is weekly work intensity calculated?**
It is calculated by multiplying daily work hours by days worked per week, then adding one-fourth of the monthly overtime hours.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/work-culture-burnout-calculator](https://vinkius.com/ai-agent-connect/work-culture-burnout-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Work Culture Burnout Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `work-culture-burnout-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Work Culture Burnout Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "work-culture-burnout-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
