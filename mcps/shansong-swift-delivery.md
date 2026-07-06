# Shansong Swift Delivery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shansong-swift-delivery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Bring Shansong's fast P2P Delivery Network into your LLM. Estimate logistics routing, dispatch riders, and track locations.

## Description
Equip your AI Agents with the **Shansong (闪送)** infrastructure logic, bringing one of the fastest Point-to-Point delivery APIs locally into your environment. Through 10 dedicated management extensions, your LLMs can govern entire delivery routes, request estimates, and interact dynamically with local couriers.

### What you can do

- **Live GPS Polling** — Instruct your agent to find where the driver is currently located using `query_rider_position`
- **Dispatch Generation** — Check prices via `calculate_fee` and officially submit `create_order` payloads dynamically
- **Rider Feedback** — Cancel routing autonomously or distribute `add_tip` commands on-demand without touching administrative dashboards

### How it works

1. Sign up on the [Shansong Open Platform](https://open.ishansong.com/)
2. Register an application and note down your **Client ID**, **App Secret**, and your default **Shop ID**
3. Push these variables into Vurb. The Node extension strictly generates the `Sign` string by converting your JSON into an MD5 Hash required by their network implicitly.

### Who is this for?

- **Retail AI Support Centers** — Handle customer 'Where is my order?' queries automatically by fetching live GPS data directly in chat contexts
- **Office Coordinators** — Empower internal company slackbots to dispatch official documents point-to-point instantly


## Available Tools (10)
- **query_city_list**: Get available active operating Cities on Shansong
- **query_order_info**: Get live order status details
- **query_rider_position**: Get live GPS coordinates of the Shansong Rider
- **query_store_list**: Get available Stores within a specific City
- **submit_complaint**: Submit complaint against assigned rider
- **add_tip**: Add a tip to encourage driver pickup
- **calculate_fee**: Calculate delivery fee dynamically
- **cancel_order**: Cancel a delivery dispatch
- **confirm_goods**: Confirm the goods were successfully picked up
- **create_order**: Create a new Shansong delivery order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shansong Swift Delivery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is the rider for order SS991024?"

**🤖 AI Agent:**
> According to the `query_rider_position` API, the assigned rider is actively streaming GPS data at Latitude 34.221, Longitude 116.480.

---

**👤 You:**
> "Tip the Shansong driver on order SS111 around 50 cents."

**🤖 AI Agent:**
> Done! I pushed a 50 cents tip payload directly against order SS111 successfully augmenting the delivery priority index.


## ❓ FAQ

**Q: How is the Shansong API payload encrypted?**
Instead of demanding complex LLM scripting to assemble `clientId`, JSON stringification, and MD5 encoding, this plugin seamlessly abstracts the `sign` variable creation. All HTTP form-data bounds are strictly governed locally on the proxy instance yielding instant results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shansong-swift-delivery](https://vinkius.com/mcp/shansong-swift-delivery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shansong Swift Delivery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shansong-swift-delivery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shansong Swift Delivery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shansong-swift-delivery": {
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
