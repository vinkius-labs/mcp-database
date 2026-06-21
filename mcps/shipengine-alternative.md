# ShipEngine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipengine-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate shipping and logistics via ShipEngine — validate addresses, compare rates, and track packages directly from any AI agent.

## Description
Connect your **ShipEngine** account to any AI agent to streamline your entire shipping workflow through natural conversation.

### What you can do

- **Address Validation** — Verify domestic and international addresses to prevent delivery failures and surcharges.
- **Rate Comparison** — Get real-time shipping rates across multiple carriers to find the best price for every shipment.
- **Label Creation** — Generate and purchase shipping labels instantly, using rate-shopping strategies (cheapest, fastest, best value).
- **Package Tracking** — Monitor shipments in real-time using tracking numbers or ShipEngine label IDs.
- **Carrier Management** — List connected carriers, connect new accounts, and manage balances for seamless operations.
- **Manifesting** — Create manifests and SCAN forms for carrier pickups directly from your agent.

### How it works

1. Subscribe to this server
2. Enter your ShipEngine API Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly compare shipping costs and generate labels without manual data entry or switching tabs.
- **Logistics Teams** — track multiple packages and validate customer addresses directly from the chat interface.
- **Developers** — test shipping workflows and carrier integrations using natural language instead of manual API calls.


## Available Tools
- **add_funds**: Add funds to a carrier balance
- **connect_carrier**: Connect a carrier account
- **create_label_rate_shopper**: Create a label using the rate shopper
- **create_label**: Create a shipping label
- **create_manifest**: Create a manifest (e.g., USPS SCAN form)
- **create_shipment**: Requires carrier_id, service_code, ship_to, and ship_from.

Create a new shipment
- **get_rates**: Calculate shipping rates
- **list_carriers**: List connected carriers
- **list_labels**: List shipping labels
- **track_label**: Track a package by label ID
- **track_package**: Track a package by carrier code and tracking number
- **validate_addresses**: Max 250 addresses.

Validate shipping addresses
- **void_label**: Void a shipping label


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipEngine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this shipping address: 4009 Marathon Blvd, Austin, TX 78756."

**🤖 AI Agent:**
> I've validated the address. It is a valid residential address in Austin, Texas. ShipEngine has confirmed the formatting is correct for delivery.

---

**👤 You:**
> "Get shipping rates for a 2lb package from Zip 90210 to 10001."

**🤖 AI Agent:**
> I found several rates for your shipment. The cheapest option is USPS Ground Advantage at $8.45, while the fastest is FedEx Overnight at $42.10. Would you like to create a label for one of these?

---

**👤 You:**
> "Track my UPS package with tracking number 1Z9999999999999999."

**🤖 AI Agent:**
> The UPS package is currently 'In Transit'. It was last scanned at the Louisville, KY hub and is estimated to be delivered by tomorrow at 7:00 PM.


## ❓ FAQ

**Q: Can I validate multiple addresses at once to avoid shipping surcharges?**
Yes! Use the `validate_addresses` tool. You can provide an array of address objects, and the agent will return validation results for up to 250 addresses in a single request.

**Q: How does the AI choose the best shipping rate for me?**
You can use the `create_label_rate_shopper` tool with a specific strategy: 'cheapest', 'fastest', or 'best_value'. The agent will automatically compare rates across your carriers and purchase the label that fits your criteria.

**Q: Can I track a package if I only have the tracking number and carrier code?**
Absolutely. Use the `track_package` tool by providing the `carrier_code` (e.g., 'ups', 'fedex') and the `tracking_number`. The agent will retrieve the latest status and location updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipengine-alternative](https://vinkius.com/mcp/shipengine-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShipEngine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shipengine-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShipEngine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipengine-alternative": {
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
