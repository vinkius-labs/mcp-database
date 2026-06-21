# ThoughtSpot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thoughtspot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search and analyze business data by interacting directly with your ThoughtSpot metadata and Liveboards via your AI agent.

## Description
Connect your **ThoughtSpot** instance to any AI agent and bring your analytics workflows directly into your chat. Search through your metadata, access reports, and list configurations natively.

### What you can do

- **Metadata Search** — Search for specific analytical assets across your organization and filter by type (Liveboards, Answers, Logical Tables)
- **Browse Visualizations** — List all available Liveboards (dashboards) and Answers (individual charts/tables) without leaving your environment
- **Team Management** — Retrieve lists of registered account users and user groups, along with their access levels
- **Backend Topologies** — List all configured data source connections (such as Snowflake and BigQuery) serving your platform
- **Organization** — Navigate through metadata tags used for classifying data objects and reports

### How it works

1. Subscribe to this server
2. Enter your ThoughtSpot Cloud Host URL, Username, and Secret Key
3. Begin asking your AI agent about your business intelligence infrastructure natively

### Who is this for?

- **Data Engineers** — Verify which backend database connections are currently active without checking the UI
- **Analytics Managers** — Look up available Liveboards, tags, and data views quickly
- **IT Admins** — Interrogate the user directory and group distributions directly from the command line or chat


## Available Tools
- **search_metadata**: Supported types include LIVEBOARD, ANSWER, LOGICAL_TABLE, etc.

Search for metadata objects in ThoughtSpot by type
- **list_liveboards**: Lists all available Liveboards (dashboards)
- **list_answers**: Lists all saved Answers (individual charts or tables)
- **list_account_users**: Lists all users in the ThoughtSpot instance
- **list_user_groups**: Lists all user groups
- **list_data_connections**: g., Snowflake, BigQuery) are connected.

Lists configured data source connections
- **list_metadata_tags**: Lists all tags used for classifying metadata objects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThoughtSpot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a list of all active database connections."

**🤖 AI Agent:**
> I found 2 data connections active on your ThoughtSpot instance:
- Connection ID: 6223-bd7-snow, Name: 'Snowflake Production Warehouse'
- Connection ID: 4422-bc5-aws, Name: 'AWS Redshift Archival'

---

**👤 You:**
> "Can you list all the user groups configured?"

**🤖 AI Agent:**
> Your ThoughtSpot environment currently has 4 logical groups:
1. 'Administrators'
2. 'Finance Viewers'
3. 'Marketing Edit'
4. 'All Users'


## ❓ FAQ

**Q: Where do I get my ThoughtSpot Secret Key?**
You can find or generate your Secret Key in the ThoughtSpot instances under the **Develop** menu, inside the **Security settings** (specifically Trusted Authentication). Note that you need admin tracking rights or developer privileges to enable this type of access.

**Q: Can the AI modify my dashboards?**
No. The integration exclusively lists and searches metadata elements (Liveboards, Data connections, Answers, Users). It will not modify, overwrite, or delete any configurations or data objects.

**Q: What types of metadata can I search for?**
Liveboards (dashboards), Answers (individual charts and tables), Logical Tables, data source connections, users, user groups, and organizational tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thoughtspot](https://vinkius.com/mcp/thoughtspot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThoughtSpot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `thoughtspot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThoughtSpot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thoughtspot": {
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
