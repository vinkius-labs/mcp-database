# DPD MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dpd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Streamline your logistics and shipping with DPD.

## Description
This MCP server integrates DPD services, allowing you to create shipments, track parcel statuses, and find nearby pickup points. It's designed for businesses that need to automate their shipping workflows efficiently.


## Available Tools
- **cancel_shipment**: Cancel an existing DPD shipment
- **create_shipment**: Provide shipment data as a JSON string.

Create a new shipment and generate parcel numbers/labels
- **find_parcelshop**: Search for DPD Pickup points (ParcelShops) near a location
- **get_labels**: Retrieve the labels for a specific shipment
- **get_manifest**: Generate or retrieve a manifest for a shipment
- **get_parcel_status**: Retrieve the tracking status for a specific parcel number
- **get_shipment_status**: Get the current status and tracking history of a shipment
- **list_countries**: List supported countries for DPD shipping
- **list_products**: List available DPD products and services
- **list_shipments**: Supports filtering by date or status. Provide filters as a JSON string.

List recent shipments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DPD** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of parcel 123456789."

**🤖 AI Agent:**
> I'm checking the current status for you.

---

**👤 You:**
> "Find DPD pickup points in Berlin."

**🤖 AI Agent:**
> Searching for nearby parcel shops...

---

**👤 You:**
> "Create a shipment from London to Paris."

**🤖 AI Agent:**
> Let's set up the shipment details.


## ❓ FAQ

**Q: How do I get DPD API credentials?**
You must be a contracted DPD client. Contact your local DPD account manager to request API access and credentials.

**Q: Which regions are supported?**
This server supports DPD global REST APIs. Regional differences are handled by providing the appropriate Base URL for your region.

**Q: Can I cancel a shipment?**
Yes, you can cancel a shipment using its ID as long as it hasn't been picked up or processed beyond a certain stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dpd](https://vinkius.com/mcp/dpd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DPD** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dpd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DPD** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dpd": {
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
