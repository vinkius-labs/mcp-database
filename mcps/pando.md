# Pando MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pando)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Share large files and folders securely with clients using branded transfer portals and download analytics for creative teams.

## Description
Connect your **Pando** account to any AI agent and take full control of your transport management system (TMS) and fulfillment orchestration through natural conversation. Pando provides a world-class platform for logistics visibility, and this integration allows you to retrieve shipment metadata, manage vehicle indents, and monitor warehouse locations directly from your chat interface.

### What you can do

- **Shipment & Carrier Orchestration** — List all managed shipments and retrieve detailed status metadata programmatically to ensure your logistics pipeline is always synchronized.
- **Vehicle Indent Tracking** — Access and monitor your vehicle placement requests (indents) directly from the AI interface to optimize fleet allocation and reduce lead times.
- **Location & Warehouse Intelligence** — List and search through your master locations and warehouses via natural language to maintain a clear overview of your supply chain nodes.
- **Material & Inventory Control** — Access your registered materials database and retrieve unit metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage shipment history to ensure your fulfillment operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pando TMS API Token from your profile settings
3. Start managing your logistics operations from Claude, Cursor, or any MCP-compatible client

No more manual spreadsheet tracking for vehicle placement. Your AI acts as a dedicated logistics coordinator or supply chain analyst.

### Who is this for?

- **Logistics Managers** — quickly retrieve shipment summaries and monitor vehicle availability without switching apps.
- **Supply Chain Planners** — automate the management of vehicle indents and track material movement via natural conversation.
- **Operations Teams** — streamline the retrieval of location metadata and monitor organizational fulfillment health directly within the chat.


## Available Tools
- **create_indent**: Pass data as a JSON string.

Create a new vehicle indent
- **get_indent_details**: Get details for a specific indent
- **get_shipment_details**: Get specific shipment details
- **check_api_status**: Verify Pando API connectivity
- **list_carriers**: List all transport carriers
- **list_indents**: List all vehicle indents
- **list_locations**: List all warehouse locations
- **list_materials**: List all registered materials
- **list_routes**: List all configured routes
- **list_shipments**: List all Pando shipments
- **list_vehicles**: List all registered vehicles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pando** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active shipments in my Pando account."

**🤖 AI Agent:**
> I've retrieved your shipments. You have 5 active deliveries, including 'Shipment #202' with Global Logistics (Status: In Transit). Which one would you like to see more details for?

---

**👤 You:**
> "Show me all available carriers and their fleet capacity for the Mumbai to Delhi route."

**🤖 AI Agent:**
> 4 carriers operate the Mumbai-Delhi corridor. "TransLogix" has 12 vehicles available (8 trucks, 4 trailers) with 96% on-time delivery. "FastFreight" offers 8 vehicles with competitive pricing at Rs 45,000 per trip. "NationalHaulers" has 15 vehicles and the best capacity. "ExpressWay" specializes in temperature-controlled shipments with 5 reefer trucks.

---

**👤 You:**
> "Create a new vehicle indent request for 3 trucks from Delhi warehouse to Jaipur hub for tomorrow."

**🤖 AI Agent:**
> Indent request created successfully (ID: IND-8923). 3 trucks requested for Delhi Warehouse to Jaipur Hub, scheduled for May 14th at 6:00 AM. Vehicle type: 20-ft closed body. Estimated transit time: 6 hours. The system has notified 4 registered carriers on this route for bid responses within the next 2 hours.


## ❓ FAQ

**Q: Can my AI automatically find the status for a specific shipment by its ID?**
Yes! Use the `get_shipment` tool with the Shipment ID. Your agent will respond with complete metadata, including carrier name, current stage, and expected delivery dates in seconds.

**Q: How do I find my Pando TMS API Token?**
Log in to your Pando TMS dashboard, navigate to your Profile or Developer settings, and you will find your unique secret token under the 'API Info' section.

**Q: What is a vehicle 'indent'?**
An indent is a formal request within the Pando platform to assign a specific vehicle for a shipment. You can track their lifecycle from placement to fulfillment via the AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pando](https://vinkius.com/mcp/pando)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pando** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pando` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pando** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pando": {
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
