# DISQO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/disqo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage consumer insight projects, track audiences, and monitor behavioral metrics via the DISQO API.

## Description
Integrate **DISQO**, the leading consumer insights and behavioral data platform, directly into your AI workflow. Manage your research projects, monitor real-time consumer trends and behavioral metrics, and track your audience panels and surveys using natural language.

### What you can do

- **Research Oversight** — List and retrieve detailed settings and execution statuses for all your consumer insight projects.
- **Behavioral Intelligence** — Access available behavioral metrics and data points tracked by the DISQO platform.
- **Audience Management** — Monitor defined research audiences, including demographic filters and panel sizes.
- **Insight Tracking** — Retrieve processed consumer insights and performance reports directly via chat.

### How it works

1. Connect the DISQO integration to your AI assistant.
2. Authorize using your DISQO API Key (found in your platform settings).
3. Orchestrate your consumer research and data analysis through intuitive conversation.

### Who is this for?

- **Market Researchers** — Quickly check project statuses and audience availability on the go.
- **Brand Strategists** — Access consumer behavioral insights and trends via chat during planning sessions.
- **Data Analysts** — Gather structured metric definitions and research data for reporting instantly.


## Available Tools
- **get_platform_metadata**: Retrieve metadata and usage limits for your DISQO account
- **get_project_details**: Get detailed settings and status for a specific DISQO project
- **quick_behavioral_audit**: Retrieve a high-level summary of the most active behavioral metrics
- **list_running_research_projects**: Identify research projects that are currently in the data collection phase
- **list_research_audiences**: List all defined consumer audiences available for research
- **list_consumer_insights**: List available consumer insights and behavioral reports
- **list_behavioral_metrics**: List behavioral metrics and data points tracked by DISQO
- **list_insight_projects**: List all consumer insight projects in your DISQO account
- **list_largest_research_panels**: Identify audience segments with the highest number of available panelists
- **search_insights_by_keyword**: Search for specific consumer insights or reports using a keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DISQO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active research projects."

**🤖 AI Agent:**
> I've found 3 active projects in your DISQO account, including 'E-commerce Trends Q3' and 'Consumer Electronics Audit'. Would you like to see the panel size for the e-commerce project?

---

**👤 You:**
> "Show me the top behavioral metrics being tracked."

**🤖 AI Agent:**
> The most active metrics in your account are 'Mobile App Engagement', 'Cross-Device Browsing Habits', and 'Search Intent Patterns'. Would you like a detailed breakdown of the 'Search Intent' data?

---

**👤 You:**
> "Which research audience has the largest panel size?"

**🤖 AI Agent:**
> The 'US-Based Millennial Shoppers' audience has the largest panel with 1.2 million verified members. The second largest is 'European Tech Enthusiasts' with 850,000 members. Should I list the demographic filters for either of these groups?


## ❓ FAQ

**Q: How do I get a DISQO API Key?**
Log in to your DISQO platform account, navigate to the API section in your organization settings, and you can generate or retrieve your unique API Key from there. Note that API access may require a specific plan.

**Q: Can the agent show real-time consumer behavior?**
Yes, you can use the list_behavioral_metrics tool to retrieve available consumer data points and high-level trends as reported by the DISQO behavioral data platform.

**Q: Is the integration secure for sensitive research data?**
Absolutely. This integration uses official DISCO API protocols and only accesses the projects and insights exposed via your API key permissions, ensuring enterprise-grade research security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/disqo](https://vinkius.com/mcp/disqo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DISQO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `disqo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DISQO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disqo": {
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
