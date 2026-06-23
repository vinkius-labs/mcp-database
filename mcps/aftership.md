# AfterShip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aftership)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Track packages worldwide — create, manage, and monitor shipments via AI.

## Description
Connect **AfterShip** tracking platform to any AI agent and track packages from 1,000+ couriers worldwide, auto-detect shipping companies, and manage all your shipments through natural language.

### What you can do

- **Package Tracking** — Create and monitor shipments from FedEx, UPS, DHL, USPS, and 1,000+ other couriers
- **Auto-Detect Courier** — Automatically identify the shipping company from just a tracking number
- **Tracking History** — View complete delivery history with checkpoint timestamps and locations
- **Delivery Management** — Mark trackings as completed, retrack expired ones, or delete old entries
- **Customer Notifications** — Set up email and SMS notifications for delivery updates
- **Courier Directory** — Browse all supported courier companies with their contact info and requirements

### How it works

1. Subscribe to this server
2. Enter your AfterShip API Key
3. Start tracking packages from Claude, Cursor, or any MCP-compatible client


## Available Tools (9)
- **create_tracking**: Requires at least the tracking number. Optionally specify the courier slug, title, customer emails, SMS phone numbers, order ID, and custom fields.

Create a new package tracking
- **delete_tracking**: This action cannot be undone.

Delete a tracking entry
- **detect_courier**: Useful when the user provides a tracking number but doesn't know which courier it belongs to. Returns a ranked list of likely couriers.

Auto-detect courier from tracking number
- **get_tracking**: Get details of a specific tracking
- **list_couriers**: ) that can be used for tracking packages.

List all supported courier companies
- **list_trackings**: Supports extensive filtering by courier (slug), tag, keyword, origin, destination, date ranges, and delivery status.

List all package trackings
- **mark_tracking_completed**: Useful when the package has been delivered but the courier hasn't updated the final status.

Mark a tracking as completed
- **retrack_tracking**: This restarts monitoring and will fetch new checkpoint updates.

Retrack an expired tracking
- **update_tracking**: Does not affect the tracking number or courier.

Update an existing tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AfterShip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track my package with tracking number 1Z999AA10123456784."

**🤖 AI Agent:**
> I've created tracking for 1Z999AA10123456784 via UPS. Status: In Transit. Latest checkpoint: Package arrived at facility in Chicago, IL on Jan 15. Expected delivery: Jan 18.

---

**👤 You:**
> "What courier handles tracking number 9400111899223344556677?"

**🤖 AI Agent:**
> Based on the tracking number format, this is most likely a USPS package (98.5% confidence). Other possibilities include DHL eCommerce (1.5%).

---

**👤 You:**
> "Show me all my active trackings."

**🤖 AI Agent:**
> You have 5 active trackings: 2 In Transit (UPS, FedEx), 1 Out for Delivery (USPS), 1 Pending (DHL), and 1 Attempted Delivery (Canada Post). The USPS package is expected to be delivered today.


## ❓ FAQ

**Q: How do I get an AfterShip API Key?**
Sign up at [**AfterShip**](https://www.aftership.com/), go to Settings > API Keys, and generate a new key. Free tier includes 100 shipments/month.

**Q: How many couriers are supported?**
AfterShip supports 1,000+ courier companies worldwide including FedEx, UPS, DHL, USPS, Royal Mail, Canada Post, Australia Post, and many regional carriers.

**Q: Can I automatically detect which courier handles my tracking number?**
Yes! Use the `detect_courier` tool with just the tracking number. It returns a ranked list of likely courier companies based on the tracking number format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aftership](https://vinkius.com/mcp/aftership)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AfterShip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aftership` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AfterShip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aftership": {
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
