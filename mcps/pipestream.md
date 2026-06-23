# PipeStream MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipestream)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Streamline real-time data flows — create streams, publish events, and fetch historical data directly from your AI agent.

## Description
Connect **PipeStream** to your AI agent to manage high-throughput data streams and event logging through natural language.

### What you can do

- **Stream Management** — List all active data channels and create new streams with custom retention policies.
- **Event Publishing** — Send JSON payloads and events to specific streams instantly.
- **Data Retrieval** — Fetch historical events from any stream with support for pagination and time-based filtering.
- **Real-time Monitoring** — Inspect the flow of data across your infrastructure without leaving your chat interface.

### How it works

1. Subscribe to this server
2. Enter your PipeStream API Key
3. Start managing your data pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check event logs and stream statuses during incident response.
- **Data Scientists** — publish experimental results or fetch sample data for analysis directly in-context.
- **Backend Developers** — verify event delivery and create new testing channels without switching to a CLI or dashboard.


## Available Tools (4)
- **create_stream**: Create a new stream
- **fetch_events**: Fetch events from a stream
- **list_streams**: List all active streams
- **publish_event**: Publish an event to a stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PipeStream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active PipeStream channels."

**🤖 AI Agent:**
> I've retrieved your active streams. You have 3 streams: 'user-signups' (ID: st_1), 'system-logs' (ID: st_2), and 'payment-events' (ID: st_3).

---

**👤 You:**
> "Create a new stream named 'production-alerts' with 48 hours retention."

**🤖 AI Agent:**
> Successfully created the stream 'production-alerts'. It is now active with a 48-hour data retention policy. The assigned Stream ID is st_99.

---

**👤 You:**
> "Fetch the last 5 events from stream st_1."

**🤖 AI Agent:**
> I've fetched the 5 most recent events from 'user-signups'. They include payload data for user registrations from the last hour. Would you like me to summarize the data?


## ❓ FAQ

**Q: Can I create a new data stream with a specific retention period?**
Yes! Use the `create_stream` tool. You can specify the name and the `retention_hours` to define how long data should be stored in that logical channel.

**Q: How do I send a JSON payload to an existing stream?**
Use the `publish_event` tool. Provide the `stream_id` and your JSON `payload`. You can also optionally include a custom ISO8601 timestamp.

**Q: Is it possible to filter events by time when fetching data?**
Absolutely. The `fetch_events` tool allows you to provide a `from_timestamp` to retrieve only the events recorded after a specific point in time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipestream](https://vinkius.com/mcp/pipestream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PipeStream** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipestream` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PipeStream** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipestream": {
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
