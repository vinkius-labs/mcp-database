# PostHog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/posthog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Analyze product data via PostHog — list insights, track persons, inspect feature flags, and monitor experiments directly from any AI agent.

## Description
Connect your **PostHog** project to any AI agent and take full control of your product analytics and feature management through natural conversation.

### What you can do

- **Insight Exploration** — List and retrieve detailed metadata for saved insights, including trends, funnels, and retention charts.
- **User Tracking** — List identified persons and inspect their properties to understand individual user behavior.
- **Feature Management** — Maintain a clear view of all feature flags and their current configurations.
- **Experiment Monitoring** — List active and past experiments to track product improvements and results.
- **Event Auditing** — List the most recent events captured by your project to verify data ingestion and user actions.

### How it works

1. Subscribe to this server
2. Enter your PostHog Personal API Key and Project ID
3. (Optional) Provide your PostHog Host (e.g., for EU instances)
4. Start analyzing your product directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check the status of a feature flag or review the results of a recent insight.
- **Growth Engineers** — monitor active experiments and user properties during development.
- **Data Analysts** — audit recent event logs and person metadata without leaving your workflow.


## Available Tools
- **get_event**: Get details for a specific event
- **get_insight**: Get details for a specific insight
- **get_person**: Get details for a specific person
- **list_actions**: List defined user actions
- **list_dashboards**: List project dashboards
- **list_events**: List recent project events
- **list_experiments**: List all active and past experiments
- **list_feature_flags**: List all feature flags
- **list_insights**: ) for the project.

List PostHog insights
- **list_persons**: List identified persons/users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PostHog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all saved insights in our PostHog project."

**🤖 AI Agent:**
> I've retrieved 12 saved insights. Some of the most recent ones are 'Daily Active Users', 'Signup Funnel', and 'Feature Adoption Trend'.

---

**👤 You:**
> "Check the status of all feature flags."

**🤖 AI Agent:**
> You have 8 feature flags. 5 are currently active (e.g., 'new-onboarding-flow', 'beta-search') and 3 are disabled.

---

**👤 You:**
> "List the last 5 persons identified in our project."

**🤖 AI Agent:**
> I've fetched the latest identified users. Here are the 5 most recent persons, including their distinct IDs and key properties like email and signup date.


## ❓ FAQ

**Q: Where do I find my Project ID?**
You can find your Project ID in PostHog under **Project Settings**. It is a numeric ID usually found at the top of the settings page.

**Q: Does this support PostHog EU instances?**
Yes! Use the optional `POSTHOG_HOST` credential and set it to `https://eu.posthog.com`. By default, it uses the US host (`https://app.posthog.com`).

**Q: Can I see individual user properties?**
Absolutely. Use the `get_person` tool with a Person ID to retrieve all properties, tags, and identification metadata for a specific user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/posthog](https://vinkius.com/mcp/posthog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PostHog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `posthog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PostHog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "posthog": {
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
