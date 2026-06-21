# Amplitude MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplitude-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track user behavior, analyze product metrics, and manage cohorts directly from your AI agent using Amplitude's powerful analytics suite.

## Description
Connect your **Amplitude** analytics account to any AI agent to ingest events, query user profiles, and analyze product performance through natural conversation.

### What you can do

- **Event Ingestion** — Send single or high-volume batch events to the Amplitude cloud using `send_events` and `send_batch_events`.
- **User Insights** — Fetch real-time user profiles, recommendations, and cohort memberships with `get_user_profile`.
- **Data Analysis** — Query segmentation metrics for specific events or export raw event data for deep analysis using `get_segmentation` and `export_data`.
- **Cohort Management** — List all behavioral cohorts or create new ones by uploading static lists of IDs with `list_cohorts` and `upload_cohort`.
- **Taxonomy & Governance** — Manage event categories, properties, and audit logs to keep your data clean and secure.

### How it works

1. Subscribe to this server
2. Enter your Amplitude API Key and Secret Key
3. Start analyzing user behavior from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — instantly retrieve event counts, check user properties, and monitor feature adoption without leaving your chat.
- **Data Analysts** — export raw data for specific time ranges and verify event taxonomy on the fly.
- **Growth Engineers** — identify users, manage cohorts, and check experiment variants directly from your development environment.


## Available Tools (21)
- **create_annotation**: Annotate charts with important dates
- **create_category**: Create a new event category (Taxonomy)
- **create_release**: Create a release to track feature impact
- **delete_users**: Submit data deletion requests (GDPR/CCPA)
- **export_data**: Export raw event data in JSON format
- **get_audit_logs**: Export administrative activity logs
- **get_experiment_variant**: Retrieve variant assignments for users (Experiment API)
- **get_segmentation**: Query metrics displayed in Amplitude charts
- **get_user_profile**: Fetch real-time user data and properties
- **group_identify**: Set or update properties for specific groups
- **identify_user**: Update user properties without sending an event
- **list_categories**: Get all event categories (Taxonomy)
- **list_cohorts**: Get all behavioral cohorts
- **list_event_properties**: Get all event properties (Taxonomy)
- **list_event_types**: Get all event types (Taxonomy)
- **list_user_properties**: Get all user properties (Taxonomy)
- **map_user**: Map one user ID to another (Global User ID)
- **send_attribution**: Send attribution data from partners
- **send_batch_events**: Send high-volume data to Amplitude (Batch API)
- **send_events**: Requires an array of event objects.

Send data directly to Amplitude (HTTP V2 API)
- **upload_cohort**: Create a cohort from a list of IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplitude** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Export raw event data from 2023100100 to 2023100123."

**🤖 AI Agent:**
> I've initiated the data export for that range. The raw event data is being retrieved from Amplitude's servers now.

---

**👤 You:**
> "Get the profile and cohort memberships for user ID 'user_123'."

**🤖 AI Agent:**
> Fetching profile for 'user_123'... This user is part of 3 cohorts: 'Power Users', 'Early Adopters', and 'Beta Testers'. Their last active property was 'premium_plan: true'.

---

**👤 You:**
> "List all behavioral cohorts in this project."

**🤖 AI Agent:**
> I found 12 behavioral cohorts. Some notable ones include 'Dormant Users' (ID: 5a2b), 'Weekly Actives' (ID: 9f1c), and 'New Signups' (ID: 3e4d).


## ❓ FAQ

**Q: Can I export raw event data for a specific time range?**
Yes. Use the `export_data` tool by providing the start and end times in YYYYMMDDTHH format to retrieve raw event data in JSON format.

**Q: How do I check which cohorts a specific user belongs to?**
You can use the `get_user_profile` tool with the specific Amplitude User ID. It will return the user's profile, recommendations, and all active cohort memberships.

**Q: Is it possible to update user properties without sending a new event?**
Yes, the `identify_user` tool allows you to set, unset, or append user properties via the Identify API without triggering a separate event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplitude-alternative](https://vinkius.com/mcp/amplitude-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplitude** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amplitude-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplitude** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplitude-alternative": {
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
