# Ship24 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ship24)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track shipments from 1200+ carriers worldwide with a universal tracking API that gives real-time delivery status updates.

## Description
Connect your **Ship24** account to any AI agent and take full control of your global logistics tracking and parcel orchestration through natural conversation. Ship24 provides a premier multi-carrier tracking API, and this integration allows you to create trackers, monitor real-time delivery progress, and search through thousands of couriers directly from your chat interface.

### What you can do

- **Parcel & Tracking Orchestration** — Create and manage parcel trackers programmatically to keep your delivery pipeline synchronized.
- **Real-time Status Intelligence** — Retrieve detailed tracking results for specific trackers, including milestones and location history directly from the AI interface.
- **Synchronous Tracking Control** — Perform instant tracking lookups for any tracking number and courier code using simple AI commands.
- **Courier & Logistics Discovery** — List and search through thousands of supported couriers to find the correct tracking provider via natural language.
- **Operational Monitoring** — Track system health and manage bulk trackers to ensure your logistics orchestration is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Ship24 API Key from your dashboard
3. Start managing your global parcel tracking from Claude, Cursor, or any MCP-compatible client

No more wrestling with multiple carrier websites to find your packages. Your AI acts as a dedicated logistics coordinator or customer support assistant.

### Who is this for?

- **Logistics Managers** — quickly retrieve parcel statuses and monitor courier performance without switching sites.
- **Customer Success Teams** — automate the retrieval of tracking details for client inquiries via natural conversation.
- **Growth Engineers** — integrate multi-carrier tracking capabilities into custom AI-driven supply chain workflows.


## Available Tools
- **create_bulk_trackers**: Bulk start tracking
- **create_tracker**: Start tracking package
- **delete_tracker**: Stop tracking package
- **get_api_status**: Get API connectivity
- **get_tracking_results**: Get package status
- **list_bulk_trackers**: List bulk shipments
- **list_couriers**: List supported carriers
- **list_active_trackers**: List all trackers
- **get_live_tracking**: Live package update
- **find_tracker_by_number**: Lookup by tracking number
- **search_couriers**: g. FedEx, Correios).

Find carrier codes
- **update_tracker_info**: Update tracker metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ship24** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track the package with tracking number '1234567890' using Ship24."

**🤖 AI Agent:**
> I've retrieved the tracking status. Your package is currently 'In Transit' in London, UK, and was last updated 2 hours ago. Would you like the full milestone history?

---

**👤 You:**
> "Find the carrier code for DHL."

**🤖 AI Agent:**
> Searching couriers... I found the identifier 'dhl' for DHL Express and 'dhl-global-mail' for DHL Global Mail. Which one would you like to use for tracking?

---

**👤 You:**
> "List all my active trackers in Ship24."

**🤖 AI Agent:**
> Retrieving your trackers... You currently have 3 shipments being monitored. The most recent is tracker 'TRK-9921' (Out for delivery). Would you like to see details for the others?


## ❓ FAQ

**Q: Can my AI automatically find the tracking status of a specific package just by providing the tracking number?**
Yes! Use the `get_live_tracking` tool with the tracking number. Your agent will respond with the real-time status, carrier info, and current location in seconds.

**Q: How do I search for a specific carrier code (e.g. FedEx or DHL)?**
Simply ask the agent to run the `search_couriers` action with the name of the carrier. It will retrieve the correct identifier for that provider.

**Q: How do I find my Ship24 API Key?**
Log in to your Ship24 account, navigate to the **Dashboard**, and select **API** to copy your unique secret API key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ship24](https://vinkius.com/mcp/ship24)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ship24** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ship24` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ship24** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ship24": {
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
