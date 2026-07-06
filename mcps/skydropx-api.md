# Skydropx API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skydropx-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Ship effectively across LatAm with Skydropx. Compare real-time carrier quotes, track live parcels, and draft PDF labels via prompt.

## Description
Connect your heavy lifting **Skydropx Carrier Console** to the AI core forcing smart algorithmic logistics to take over.

### What you can do

- **Order Estimations** — Feed dimensions targeting remote Zip Codes directly querying real-time rates crossing DHL, Estafeta, and FedEx in just seconds.
- **Label Manipulation** — List and filter active PDF printing matrices representing legal postal guides to dispatch trucks.
- **Cancel Bloats** — Did you mistype a zip code? Just ask to cancel an unprinted label fetching an instant native refund to your balance.
- **Radar Tracking** — Pull live way-point telemetry for a specific tracking number to handle mad clients seamlessly.

### How it works

1. Append the generic node
2. Introduce your API token bound directly from Skydropx Web parameters natively mapped.
3. Talk to Claude commanding heavy boxes logically.

### Who is this for?

- **Mexican eCommerces** — Seeking full command of shipments directly crossing digital storefront bounds bridging API checks.
- **Logistics Agents** — Constantly searching tracking nodes tired of visiting massive portals.
- **Operations Leads** — Checking real-time shipping costs blindly quoting items scaling up.


## Available Tools (12)
- **create_label**: Purchase and generate a printing label
- **create_package**: Register a new package format
- **create_shipment**: Draft a brand new shipment record
- **get_quotation**: Quotate shipping carrier rates
- **get_shipment**: Get a given shipment profile
- **get_tracking**: Hunt down real-time package statuses
- **list_carriers**: List synced local mail carriers
- **list_labels**: List formal logistic labels (Guides)
- **list_locations**: List registered origin warehouses
- **list_packages**: List saved standard package templates
- **list_shipments**: List active e-commerce shipments
- **cancel_label**: Void an active shipping label


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skydropx API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need to create a shipment calculation instance right now. Add a medium box weighing 2KG targeting CP '88392' in MX."

**🤖 AI Agent:**
> Request compiled correctly into Skydropx matrices! Generated internal Shipment instance. The new UUID allocated rests functionally. I am ready to jump onto pulling Native Carrier Quotes based on this profile. Do we proceed asking the fleets?

---

**👤 You:**
> "Search exactly where the package numbered 'SKY099-B' currently sits from our past dispatch."

**🤖 AI Agent:**
> Tracking network probed! Internal records show 'SKY099-B' marked strongly as [DELIVERED]. The checkpoint occurred cleanly yesterday at 14:00. The proof of signature registers 'Maria'. We closed this flawlessly over local Carrier logs.

---

**👤 You:**
> "List all origin locations"

**🤖 AI Agent:**
> Here.


## ❓ FAQ

**Q: Is it completely safe typing my Skydropx Token Key under the workspace credentials menu?**
Yes. Following standard protocol from Vinkius ecosystem, the framework utilizes an implicit `sensitive: true` marker mapping directly blocking its text input masking UI rendering perfectly from eyes.

**Q: Can I simply track a parcel giving Claude only the tracking string ID?**
Yes! Trigger dynamically `get_tracking` expressing plainly the string, and Skydropx routes heavily providing the array of checkpoints, signatures, and courier state on the payload back to you.

**Q: Is the tracking live directly?**
Yes, queries real APIs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skydropx-api](https://vinkius.com/mcp/skydropx-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skydropx API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skydropx-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skydropx API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skydropx-api": {
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
