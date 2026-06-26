# Officevibe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/officevibe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee engagement via Officevibe — track pulse survey scores, feedback, and NPS directly from your AI agent.

## Description
Connect your **Officevibe** (by Workleap) account to your AI agent and gain deep insights into your workplace culture and employee engagement through natural conversation.

### What you can do

- **Engagement Scores** — Retrieve aggregated engagement and satisfaction scores for your entire organization or specific teams.
- **Pulse Metrics** — Access granular scores for key sub-metrics like Recognition, Relationship with Manager, and Wellness.
- **Feedback Monitoring** — List qualitative survey feedback and comments, and retrieve full follow-up conversations.
- **NPS Tracking** — Monitor your current Employee Net Promoter Score (eNPS) and view historical trends.
- **User & Team Oversight** — List all employees and organization segments to understand your culture's structure.
- **Deep Inspection** — Fetch complete metadata and profile information for specific employees using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Officevibe API Key (generated in the Workleap Developer Portal)
3. Start monitoring your workplace culture from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Managers & People Ops** — quickly check engagement trends or read recent feedback without opening the dashboard.
- **Team Leads & Supervisors** — monitor your team's pulse metrics and follow up on feedback in real-time.
- **Culture Officers** — automate the retrieval of NPS and engagement data for internal culture reporting.


## Available Tools (10)
- **get_feedback_replies**: Get feedback conversation
- **get_employee_details**: Get specific employee info
- **list_user_attributes**: List custom user attributes
- **get_engagement_metrics**: g., Recognition, Relationship with Manager).

Get granular engagement metrics
- **get_engagement_scores**: Get overall engagement scores
- **get_nps_scores**: Get employee NPS scores
- **list_survey_feedback**: List survey feedback
- **list_vibe_segments**: List audience segments
- **list_vibe_teams**: List organization teams
- **list_employees**: List all employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Officevibe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current organization engagement score?"

**🤖 AI Agent:**
> Retrieving engagement scores... Your organization's current engagement score is 8.2 out of 10. The score has remained stable over the last 30 days. Would you like a breakdown of the 10 key sub-metrics?

---

**👤 You:**
> "List the latest qualitative feedback from employee surveys."

**🤖 AI Agent:**
> Fetching survey feedback... I found 5 recent comments. One employee suggested 'More healthy snacks in the breakroom' while another mentioned 'Excellent support from my manager during the launch'. Shall I retrieve the full conversation for any of these?

---

**👤 You:**
> "Show me the Employee NPS (eNPS) trend for this quarter."

**🤖 AI Agent:**
> Retrieving NPS data... Your current eNPS is +45, which is considered 'Excellent'. The trend shows a steady climb from +38 at the beginning of the quarter. Would you like to see which team segment contributed most to this growth?


## ❓ FAQ

**Q: How do I get an Officevibe API Key?**
Log in to the Workleap Developer Portal (https://developer.workleap.com/) using your Officevibe credentials to create an application and generate your API key.

**Q: Is employee feedback anonymous through the API?**
Yes. Officevibe enforces the same anonymity rules through the API as it does in the dashboard. You will see the feedback text but not the identity of the employee if it is anonymous.

**Q: What metrics are included in engagement scores?**
Scores include the 10 key engagement metrics: Recognition, Feedback, Relationship with Peers, Relationship with Manager, Satisfaction, Alignment, Happiness, Wellness, Personal Growth, and Ambassadorship.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/officevibe](https://vinkius.com/mcp/officevibe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Officevibe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `officevibe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Officevibe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "officevibe": {
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
