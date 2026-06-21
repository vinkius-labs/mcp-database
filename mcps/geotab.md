# Geotab MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geotab)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Automate fleet management via Geotab — manage devices, track trips, and monitor vehicle diagnostics directly from any AI agent.

## Description
Connect your **MyGeotab** account to any AI agent to streamline your telematics and fleet operations through natural conversation.

### What you can do

- **Entity Management** — Retrieve, create, or update Devices, Users, Zones, and Rules using `get_entity`, `add_entity`, and `set_entity`.
- **Real-time Data Feeds** — Use `get_feed` for high-volume synchronization of LogRecords, StatusData, and FaultData.
- **Trip & Exception Tracking** — Query historical Trips and ExceptionEvents to analyze fleet behavior and safety compliance.
- **Batch Operations** — Execute multiple API calls in a single request with `execute_multi_call` for maximum efficiency.
- **Quick Auditing** — Get instant counts of specific records using `get_count_of` without downloading entire datasets.

### How it works

1. Subscribe to this server
2. Provide your Geotab credentials (Server, Database, Username, and Password)
3. Start managing your fleet from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — monitor vehicle health and trip history without manual report generation.
- **Developers** — integrate telematics data into workflows using natural language instead of complex SDK calls.
- **Operations Teams** — quickly audit user access and device status across large databases.


## Available Tools
- **add_entity**: Provide the full entity JSON object.

Creates a new entity in the database
- **get_count_of**: Returns the number of entities matching a search
- **get_feed**: Returns up to 50,000 records and a toVersion token for the next call.

Continuously retrieves new or updated data (incremental polling)
- **get_entity**: Retrieves a list of entities based on search criteria
- **execute_multi_call**: Provide a JSON array of call objects, each containing a "method" and "params".

Executes multiple API calls in a single HTTP request
- **remove_entity**: Deletes an entity from the database
- **set_entity**: The entity JSON must include the ID of the record being updated.

Updates an existing entity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geotab** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active devices in my Geotab database."

**🤖 AI Agent:**
> I've retrieved the list of devices. You have 12 active units, including 'Truck 01' (ID: b1) and 'Van 04' (ID: b2). Would you like to see the status data for any of them?

---

**👤 You:**
> "How many trips were recorded yesterday? Use get_count_of."

**🤖 AI Agent:**
> There were 45 trips recorded in the database for the requested period.

---

**👤 You:**
> "Get the latest feed of FaultData using get_feed."

**🤖 AI Agent:**
> I've fetched the latest FaultData feed. I found 3 new fault records, including an engine warning on 'Truck 01'. I also have the toVersion token for your next update.


## ❓ FAQ

**Q: Can I retrieve a list of all vehicles in my fleet?**
Yes! Use the `get_entity` tool with `typeName` set to 'Device'. You can also provide optional search criteria to filter by name or group.

**Q: How do I synchronize large amounts of engine data efficiently?**
For high-volume data, use the `get_feed` tool. It is designed for incremental polling of entities like `LogRecord` or `StatusData`, returning a token for the next call to ensure no data is missed.

**Q: Is it possible to perform multiple updates at once?**
Yes. The `execute_multi_call` tool allows you to batch several API methods into a single request, which is faster and more efficient for bulk operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geotab](https://vinkius.com/mcp/geotab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geotab** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `geotab` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geotab** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geotab": {
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
