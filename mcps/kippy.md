# Kippy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kippy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track GPS locations of pets and loved ones in real time with wearable devices that send alerts when they leave safe zones.

## Description
Connect your **Kippy** account to any AI agent and manage performance tracking through natural conversation.

### What you can do

- **OKR Tracking** — Browse objectives and key results with progress percentages
- **Goal Management** — Create, update, and track individual and team goals
- **Performance Reviews** — Access review cycles, feedback, and ratings
- **Team Monitoring** — Track team performance metrics and alignment
- **Progress Reports** — Generate performance summaries and trend analysis

### How it works

1. Subscribe to this server
2. Enter your Kippy API Key, Organisation ID, and Username
3. Start managing performance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Teams** — manage review cycles and performance data
- **Managers** — track team OKRs and individual goals
- **Employees** — review personal progress and feedback


## Available Tools
- **list_annual_scores**: List annual performance metrics
- **list_appraisals**: List performance reviews and appraisals
- **list_audit_logs**: List system audit logs
- **list_competencies**: List skills and competency tracking
- **list_feedback**: List feedback entries
- **list_kpi_scores**: List KPIs with their current scores
- **list_kpis**: List all KPIs for the organization
- **list_notes**: List comments and annotations
- **list_project_scores**: List projects with their current scores
- **list_projects**: List organizational projects
- **list_team_scores**: List team performance scores
- **list_teams**: List teams in the organization
- **list_users**: List users in Kippy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kippy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all OKRs for Q2 and the team members falling behind."

**🤖 AI Agent:**
> Q2 OKRs: 8 objectives. 'Increase revenue 20%' (65% ✅ on track). 'Launch mobile app' (40% ⚠️ at risk). 'Hire 10 engineers' (80% ✅). Behind: 3 people. Sarah — 'Mobile app MVP' (25%, deadline May 15). Mike — 'API documentation' (30%). Lisa — 'Customer onboarding' (35%).

---

**👤 You:**
> "Show the latest performance review cycle and ratings."

**🤖 AI Agent:**
> Q1 Review Cycle: 35 employees reviewed. Completion: 92% (3 pending). Ratings: Exceptional (4), Exceeds (12), Meets (15), Below (3), Needs Improvement (1). Average: 3.4/5. Top: Sarah Chen (4.8/5), Mike Torres (4.6/5). Pending: James, Lisa, David.

---

**👤 You:**
> "Create a new goal for the Engineering team and track alignment."

**🤖 AI Agent:**
> Goal created! 'Reduce API response time to <100ms' — Team: Engineering, Owner: Sarah, Deadline: Jun 30. Key Results: 1) Optimize DB queries (0/100%). 2) Implement caching (0/100%). 3) Load testing passing (0/100%). Alignment: Maps to company OKR 'Improve platform performance'. Engineering alignment: 85% (6 of 7 goals linked).


## ❓ FAQ

**Q: Can I track OKRs and goal progress?**
Yes. Browse all objectives with key results and progress percentages. Create new goals, update progress, and track alignment across teams.

**Q: Does Kippy require multiple credentials?**
Yes. Kippy requires three credentials: **API Key**, **Organisation ID**, and **Username**. All are used for authentication against `kippy-tsc.appspot.com/api`.

**Q: Can I access performance reviews and feedback?**
Yes. Browse review cycles, access individual feedback and ratings, and monitor completion status across the organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kippy](https://vinkius.com/mcp/kippy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kippy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kippy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kippy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kippy": {
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
