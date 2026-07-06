# Kissmetrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kissmetrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track user behavior, set properties, and query analytics data via the Kissmetrics API.

## Description
Connect your **Kissmetrics** account to any AI agent to automate your user behavioral analytics and tracking workflows. This MCP server enables your agent to record events, manage user properties, and query complex metric data directly from natural language interfaces.

### What you can do

- **Behavior Tracking** — Record custom events for specific users to monitor their journey and interactions
- **Profile Management** — Set and update user properties and metadata to maintain rich customer profiles
- **Identity Resolution** — Alias multiple identities to maintain a single, unified view of a user across sessions
- **Data Discovery** — List all defined event types and property names currently in your account
- **Analytical Querying** — Retrieve people counts and metric values over time to track business performance

### How it works

1. Subscribe to this server
2. Enter your Kissmetrics API Key
3. Start managing your behavioral data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — Monitor feature adoption and user engagement trends via natural language commands
- **Growth Marketers** — Quickly track campaign conversions and segment user behaviors without writing code
- **Developers** — Integrate server-side event tracking and data retrieval into your development workflow


## Available Tools (7)
- **alias_identities**: g., linking a browser ID to an email).

Link two identities together
- **list_event_types**: List all event types defined in the account
- **list_property_names**: List all property names used in the account
- **query_people_count**: Get the count of people matching specific criteria
- **query_metric_data**: Requires a metric ID and query parameters.

Get data for a specific metric
- **record_event**: Requires a person identity (email/ID) and an event name.

Record a behavior event for a person
- **set_person_properties**: Set properties for a specific person


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kissmetrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a 'Purchased' event for 'user@example.com' with price 49.99."

**🤖 AI Agent:**
> I've recorded the 'Purchased' event for user@example.com. The price of 49.99 has been successfully attached as a property to this event in Kissmetrics.

---

**👤 You:**
> "Set the property 'Plan Tier' to 'Enterprise' for 'customer_123'."

**🤖 AI Agent:**
> Successfully updated properties for customer_123. The 'Plan Tier' is now set to 'Enterprise' in their behavioral profile.

---

**👤 You:**
> "Show me all event types defined in my account."

**🤖 AI Agent:**
> I've retrieved 15 event types from your Kissmetrics account, including 'Signed Up', 'Logged In', 'Purchased', and 'Feature Used'. Would you like to query metrics for any of them?


## ❓ FAQ

**Q: How do I identify a person in Kissmetrics?**
You can use an email address or any unique string as the identity (`person` parameter) in the tracking tools. Use the `alias_identities` tool to link multiple IDs to the same person.

**Q: Can I query report data through this agent?**
Yes, you can use the `query_metric_data` or `query_people_count` tools to retrieve aggregated values and counts based on your collected behavioral data.

**Q: Is it possible to see all my custom events?**
Absolutely. Use the `list_event_types` tool to retrieve a comprehensive list of all events that have been defined or recorded in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kissmetrics](https://vinkius.com/mcp/kissmetrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kissmetrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kissmetrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kissmetrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kissmetrics": {
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
