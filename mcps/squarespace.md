# Squarespace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/squarespace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI with read-only superpowers over your Squarespace platform. Scan transactions, track orders, and audit inventory effortlessly.

## Description
Ingest the heartbeat of your **Squarespace** properties directly into your AI workspace context utilizing a strictly readable auditing layer. Replace messy manual navigation hunting down tracking numbers or customer profiles in browser windows. Through pure conversational AI logic, command vast scans pulling your entire catalog of items, compiling customer databases or digesting active transaction ledgers locally in plain text.

### What you can do

- **Order Diagnostics** — Review your unfulfilled and processed shipment queue invoking `list_orders` sweeping up lists to inspect specific line items demanding `get_order_details`
- **Financial Ledgers** — Extract global financial movements pulling down clean transaction strings calling the `list_transactions` tool
- **Catalog & Stock Surveillance** — Sweep the merchandising parameters pulling global shop structures via `list_products` and assessing available balances requesting `list_inventory`
- **CRM Exporting** — Harvest an active listing mapping your contacts natively pushing text via `list_member_profiles` directly into Cursor or Claude

### How it works

1. Spark the connection engine initiating this read-only MCP module
2. Securely pass your overarching Developer API Key inside the host
3. Engage your language model requesting an unstructured breakdown table reporting your lowest stock items automatically

### Who is this for?

- **Marketing Data Scientists** — synthesize massive databases filtering buyer trends extracting demographics from `list_member_profiles` natively via AI summarization
- **Back-Office Administrators** — eliminate platform hopping; easily identify if John Doe paid his balance simply questioning the bot to check `list_transactions`
- **Founders & Owners** — audit operational e-commerce status maintaining rigorous read-only peace of mind without worrying about the AI making fatal destructive modifications


## Available Tools (6)
- **list_inventory**: Lists inventory levels for products
- **get_order_details**: Retrieves details for a specific order
- **list_orders**: Lists Squarespace commerce orders
- **list_products**: Lists all products in the store
- **list_member_profiles**: Lists member or customer profiles
- **list_transactions**: Lists financial transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Squarespace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pull down my customer profiles list. I want to see if any users are from Canada natively mapped resolving via MCP tools."

**🤖 AI Agent:**
> Pulling data utilizing direct pipeline `list_member_profiles`. Scanned 14 overall valid active objects retrieved and loaded internally. 

**Filtered Result**: I have detected 2 profiles with a shipping/contact locale mapped to Canada ('CA'):
- **Alice Vancouver (alice.v@mail.com)** | ID: P#98s0s1
- **Jean L. (jean.l@domain.ca)** | ID: P#001aX1

I can expand their full line item purchase history tracking backwards if needed.

---

**👤 You:**
> "Use the transaction readout scanner to count how many completely refunded logs appear in the last batch."

**🤖 AI Agent:**
> Cycling payload natively engaging `list_transactions` auditing backend ledgers internally...

Found **42** recent transactions stored loosely across internal responses. After analyzing inner data vectors, **3 transactions** possess fully executed refund events explicitly attached holding values returned to the buyer payload:

1. **Tx_abc123** ($40.00 | Jan 02)
2. **Tx_zzz009** ($15.00 | Jan 04)
3. **Tx_plx444** ($120.50 | Jan 10)

All remaining logs read normal processed settled positive values.


## ❓ FAQ

**Q: Is there any risk of the AI accidentally deleting or corrupting my live Squarespace products?**
No. This tool operates exclusively in a secure 'Read-Only' capacity. It can only ingest matrices and extract data from existing records mapping to tools like `list_products` or `list_orders`. It does not possess foundational modules to execute POST or DELETE endpoints.

**Q: Wait, so I can fetch orders but I cannot ship them using this specific integration right?**
Exactly. This version is designed entirely for read operations safeguarding users managing analytical reports. If you need powerful backend modification logic (like dispatching orders), implement the 'Squarespace Commerce' MCP package instead.

**Q: Do I need any specialized third-party proxy tools to make this connect to Squarespace?**
No extra software. The integration passes traffic straight calling the official native Squarespace API channels endpoints connecting symmetrically to your environment 1:1 using only your standard Bearer key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/squarespace](https://vinkius.com/mcp/squarespace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Squarespace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `squarespace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Squarespace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "squarespace": {
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
