# Clip API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clip-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate Mexico's leading payment gateway via Clip — generate payment links, manage refunds, and track settlements seamlessly via AI.

## Description
Directly empower your intelligent agents with the **Clip API**, the undisputed champion of point-of-sale and card payment gateways across Mexico. Bypass clunky merchant dashboards by commanding 10 specialized financial tools built to execute transactions, force refunds, and reconcile bulk backend settlements securely through plain text.

### What you can do

- **Payment Link Generation** — Programmatically spin up highly secure payment links instantly firing off collection demands mapped directly to specific user workflows without manual UI clicks.
- **Transaction Auditing** — Track pending authorizations scanning exact balances sniffing out potential fraud drops analyzing transaction statuses aggressively.
- **Automated Reconciliations** — Pull bulk settlement reports extracting clean matrices charting precisely when cash pipelines hit your registered banks.
- **Inventory & Subscription** — Manage deep catalog arrays syncing SKUs and dictating heavy recurring billing cycles charging Mexican cards passively.

### How it works

1. Solidify your merchant approval inside the [Clip Developer Terminal](https://developer.clip.mx/)
2. Navigate toward the backend isolating and grabbing your pure **API Key** credentials
3. Slide the key firmly into the vault perimeter below completely locking the environment
4. Cast commands directly! Vurb autonomously absorbs the REST payloads mutating heavy JSON demands into simple conversational actions continuously securely.

### Who is this for?

- **LatAm Finance Managers** — force comprehensive settlement extractions cross-checking physical terminal collections against real bank drops directly via chat.
- **Support Operations** — validate card payment denials and orchestrate instantaneous full or partial refunds for furious customers securely answering support tickets.
- **E-Commerce Architects** — hard-sync inventory SKUs marrying Clip catalogs identically with dynamic web-stocks bypassing heavy manual imports saving thousands of clicks.


## Available Tools (10)
- **add_product_to_catalog**: Add a new item to the Clip Point of Sale catalog
- **cancel_payment_link**: Void an active payment link
- **create_payment_link**: Generate a Clip payment link to charge customers via card
- **create_subscription_plan**: Build a recurring billing cycle charging clients periodically
- **get_balance_summary**: Retrieve cash balance awaiting settlement
- **get_settlement_reports**: Fetch detailed historical settlement reports
- **get_transaction_status**: Retrieve the status of a payment transaction
- **list_products_catalog**: Pull the complete inventory catalog registered in Clip
- **list_terminals**: List all registered physical POS Clip terminals
- **refund_transaction**: Omit amount for full refund.

Execute a full or partial refund for a settled transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clip API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a new custom MXN payment link exactly for 450.50 referenced as invoice #X-99T."

**🤖 AI Agent:**
> Clip transaction mechanism engaged! I have fully generated the MXN 450.50 payment gateway link. The URL is 'https://pay.clip.mx/x99t'. It's currently active and awaiting funds capture. Shall I send it to the client via SMS logic?

---

**👤 You:**
> "Refund the latest transaction specifically identified as Txn_88Z to its origin card fully."

**🤖 AI Agent:**
> Initiating vault rollback command targeting specific Clip Txn_88Z block... Full Refund sequence finalized successfully avoiding secondary validations cleverly. The entire volume will appear on the customer's bank statement cleanly within 48 to 72 business hours. Need any more void actions handled natively?

---

**👤 You:**
> "Calculate my comprehensive real cash balance available anticipating the incoming bulk settlements today blindly."

**🤖 AI Agent:**
> Sweeping internal Clip balances... I calculate MXN 35,490.20 actively marked as 'Settled' and available for your incoming sweep to the pre-registered Banamex account within the next 14 hours automatically without intervention. You also hold 4,000 pending. Shall I print the daily CSV?


## ❓ FAQ

**Q: Can I automatically refund payments without ever navigating to the Clip website?**
Yes. The `refund_transaction` interface executes server-side cryptographic voiding. Pass the definitive transaction ID alongside an optional amount override, and the refund logic routes directly through Clip's banking partners unconditionally.

**Q: Are the payment links generated permanent or do they have expiration windows?**
By default, Payment links created via this endpoint remain actively valid until either paid successfully or explicitly halted. You can seamlessly use the `cancel_payment_link` tool to kill rogue links manually blocking external vulnerability loopholes.

**Q: Can the agent check if physical POS terminals are active and connected to my account?**
Yes. The `list_terminals` endpoint fetches the fleet array directly from Clip servers. It outputs device IDs mapped to your registry ensuring no unauthorized POS physical readers are leeching payments stealthily.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clip-api](https://vinkius.com/mcp/clip-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clip API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clip-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clip API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clip-api": {
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
