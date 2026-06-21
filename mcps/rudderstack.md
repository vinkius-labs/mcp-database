# RudderStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rudderstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Connect your AI assistant natively to RudderStack to effortlessly monitor global data sources, trace routing connections, and audit enterprise marketing audiences via structured text commands.

## Description
Connect your conversational assistant directly into **RudderStack**, the leading enterprise Customer Data Platform (CDP) dedicated to developers. This integration robustly morphs your AI into a dynamic data engineer, enabling smooth real-time conversational audits encompassing configured sources, end tracking pipeline connections, tracking plans, and segmentation.

### What you can do

- **Explore Inlets and Outlets** — Command the assistant directly natively to list every active data intake platform (`list_sources`) securely or drill flawlessly deep into individual setup environments using detailed metrics (`get_source`). View every downstream endpoint gracefully (`list_destinations`).
- **Audit Data Interconnectivity** — Are the web analytics pipelines correctly tied proactively to the respective data warehouses? The AI natively verifies data pipeline flows mapping seamlessly directly (`list_connections`).
- **Governance & Audience Mapping** — Instantly review strict operational event typing mappings natively securely configured (`list_tracking_plans`), or query active personalized remarketing sub-clusters synced locally to customer databases cleanly natively (`list_audiences`).

### How it works

1. Successfully inject the RudderStack operational connector seamlessly inside your secure active MCP workspace cleanly natively.
2. Sign in seamlessly directly into your enterprise cloud data CDP account correctly mapped online. Navigate strictly inside your Settings panel properly natively finding 'Personal Access Tokens'.
3. Extract this API code thoroughly securely strictly pasting this encrypted `RudderStack Access Token` organically seamlessly inside the form directly natively mapped strictly below.
4. Interact effectively strictly natively strictly cleanly: "Show me natively exactly what data sources correctly actively dynamically connect organically natively to the primary active cloud destination node."

### Who is this for?

- **Data Engineers** — Perform seamless integration checks rapidly utilizing basic humanly typed verbiage seamlessly pulling accurate identifiers correctly parsing perfectly efficiently.
- **Marketing Integrators** — Fetch precise data schemas visually organically mapping custom internal events organically continuously parsing intelligently globally tracking properly seamlessly seamlessly flawlessly correctly internally.
- **Enterprise Administrators** — Dynamically assess overall flow operations safely locally organically properly strictly properly optimally correctly seamlessly perfectly strictly cleanly simply gracefully organically purely natively gracefully.


## Available Tools
- **get_destination**: Retrieves details for a specific data destination
- **get_source**: Retrieves details for a specific data source
- **list_audiences**: Lists all defined user audiences
- **list_connections**: Lists all source-to-destination connections
- **list_destinations**: Lists all data destinations configured in RudderStack
- **list_sources**: Lists all data sources configured in RudderStack
- **list_tracking_plans**: Lists all tracking plans defined in the data catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RudderStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all configured sources."

**🤖 AI Agent:**
> I effectively efficiently accurately parsed internal records manually flawlessly pulling the actively mapped instances naturally gracefully seamlessly organically running `list_sources`. Your configuration optimally possesses smoothly accurately exactly 3 sources properly successfully securely effectively.

---

**👤 You:**
> "Check if the connection between our website source and Snowflake destination is active."

**🤖 AI Agent:**
> Verified: The connection (ID: conn_12345) from 'Production Website' (source) to 'Snowflake Data Warehouse' (destination) is currently active and healthy with 0 dropped events in the last hour.

---

**👤 You:**
> "Show me the tracking plans currently applied to our iOS app source."

**🤖 AI Agent:**
> The 'iOS App' source is currently linked to the 'Mobile E-commerce v2' tracking plan. This plan enforces strict schemas for 15 standard commerce events.


## ❓ FAQ

**Q: Can the AI change tracking plans or modify data source schemas directly?**
No, this integration limits actions inherently strictly internally seamlessly natively gracefully fully perfectly properly reliably securely precisely solely toward organically gracefully strictly accessing read-only operations effectively smoothly efficiently successfully parsing natively purely locally correctly efficiently safely retrieving data logically effortlessly organically reliably cleanly dynamically dynamically safely correctly reading data purely explicitly properly.

**Q: Can the AI list audience segments and their sync status?**
Yes. Use `list_audiences` to retrieve all configured audience segments, including their names and associated destination syncs. This is useful for verifying remarketing pipelines.

**Q: Which destination types does the integration support?**
The integration queries any destination configured in your RudderStack workspace — data warehouses, analytics platforms, marketing tools, and cloud storage. Use `list_destinations` to see all active endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rudderstack](https://vinkius.com/mcp/rudderstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RudderStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rudderstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RudderStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rudderstack": {
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
