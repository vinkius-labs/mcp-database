# Keen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stream events and perform powerful analytics queries via Keen.io.

## Description
Connect your **Keen.io** project to any AI agent to automate data collection and analysis. This MCP server allows your agent to record events and run complex analytical queries (count, sum, average, etc.) directly from natural language.

### What you can do

- **Event Recording** — Send custom event data to any collection in your project instantly
- **Compute Metrics** — Run aggregation queries like `count`, `sum`, and `average` on your event data
- **Data Discovery** — List all event collections, saved queries, and cached datasets
- **Insight Extraction** — Retrieve unique values for specific properties to understand data distribution
- **Project Oversight** — Get comprehensive metadata and configuration details for your Keen project

### How it works

1. Subscribe to this server
2. Enter your Keen Project ID and Master Key
3. Start streaming and analyzing data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Engineers** — Quickly test event recording and verify collection schemas via natural language
- **Product Analysts** — Run ad-hoc metrics and aggregation queries without writing code
- **Developers** — Integrate event streaming checks and project status monitoring into your development workflow


## Available Tools (10)
- **average_property**: Calculate average of a property
- **list_collections**: List all event collections
- **count_events**: Count total events in a collection
- **list_datasets**: List cached datasets
- **list_saved_queries**: List all saved queries
- **select_unique**: List all unique values for a property
- **sum_property**: Sum numeric values of a property
- **count_unique**: Count unique values for a property
- **get_project_details**: Get project configuration and details
- **record_event**: Record a single event to a collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a 'purchase' event with price 99.99 and user 'user_123' in Keen."

**🤖 AI Agent:**
> I've recorded the 'purchase' event to your Keen project. The data has been successfully sent to the 'purchase' collection.

---

**👤 You:**
> "What is the total count of 'page_view' events?"

**🤖 AI Agent:**
> I've run the query. There are a total of 15,432 events in your 'page_view' collection.

---

**👤 You:**
> "Show me all saved queries in my project."

**🤖 AI Agent:**
> I found 8 saved queries, including 'Daily-Revenue-Summary', 'User-Retention-Analysis', and 'Checkout-Conversion-Funnel'.


## ❓ FAQ

**Q: Can I record a single event using this agent?**
Yes, the `record_event` tool allows you to send a JSON object representing your event directly to any named collection.

**Q: How do I calculate the average value of a property?**
Use the `average_property` tool by specifying the collection name and the numeric target property you want to average.

**Q: Is it possible to see my project's collections?**
Absolutely. The `list_collections` tool retrieves a list of all event types (collections) currently stored in your Keen project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keen](https://vinkius.com/mcp/keen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keen": {
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
