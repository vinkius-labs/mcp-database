# PayPal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paypal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage e-commerce payments via PayPal — orchestrate orders, process captures securely, issue refunds natively, and structure active subscriptions using AI.

## Description
Equip your generative intelligent instances with strict orchestration boundaries mapped directly over the **PayPal E-Commerce API**. Programmatically instantiate checkout orders natively, process authorized status checkpoints, execute hard refunds securely bounding financial arrays implicitly, and parse subscription structures dynamically fetching continuous log parameters seamlessly.

### What you can do

- **Order Fulfillment** — Trace strict lifecycle bounds generating orders natively or querying parameters securely verifying their complete operational states
- **Financial Capture Pipelines** — Dispatch logical constraints executing authorized commands actively processing captures into verified merchant limitations structurally
- **Refund Logistics** — Enforce operational arrays pushing robust limits explicitly commanding refunds against logged Capture IDs verifying logic dynamically
- **Subscription Trees** — Extract limits evaluating metadata nodes parsing active billing loops over recurring setups strictly using parameters asynchronously

### How it works

1. Subscribe configuring boundaries natively to an AI model dynamically (like Claude)
2. Add your precise PayPal bounded Sandbox/Live Client ID explicit parameter and Secret credentials securely
3. Start dispatching explicit explicit financial payloads modeling real arrays effortlessly natively

### Who is this for?

- **Software Engineers** — configure and validate staging checkout responses locally identifying object outputs without switching to sandbox dashboards
- **Financial Operations** — evaluate capture loops issuing explicit refunds testing complex ledger logic natively across endpoints
- **Customer Success** — query dynamic user bounds inspecting exactly whether a recurring subscription object is logistically 'Active' locally directly inside chat


## Available Tools (10)
- **authorize_order**: Authorize payment for an order
- **capture_order**: Capture payment for an order
- **create_order**: Create a new PayPal checkout order
- **cancel_subscription**: Cancel an active subscription
- **capture_authorization**: Capture a previously authorized payment
- **get_order_details**: Get details for a specific order
- **get_subscription**: Get details for a recurring subscription
- **refund_capture**: Refund a captured payment
- **suspend_subscription**: Suspend an active subscription
- **void_authorization**: Void an existing authorization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PayPal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a strictly bounded new order array configuring explicit amounts totaling 50.00 USD."

**🤖 AI Agent:**
> Invoked natively checking payload bounds. Operation success encapsulating order explicitly. Returned native Order ID is '98xx23'. Financial bounds verified natively gracefully awaiting further capture processes explicitly.

---

**👤 You:**
> "Execute native limits to capture order logically tracking specific Order ID 'xy2z9'."

**🤖 AI Agent:**
> Mapped explicit endpoints requesting execution. Payload captured parameters successfully. Final 'COMPLETED' native limit returned. The Capture ID logged is explicitly 'zz9xx82'. Check JSON array structurally if needed.

---

**👤 You:**
> "Verify explicit details mapping boundaries for the active subscribed model ID 's99a'."

**🤖 AI Agent:**
> Commanded tracking parameters hitting structural bounds `get_subscription`. Payload bounds returned efficiently. Current logical profile natively sits actively running ('ACTIVE'). Next mapped explicitly invoice limits generate safely on Sep 14.


## ❓ FAQ

**Q: Can I switch explicitly between testing (Sandbox) and Live operational arrays natively?**
Yes. The environment parameters expose an explicitly bounded flag globally allowing configuration arrays parsing seamlessly switching requests between Sandbox limits and Live endpoints. Ensure your keys correspond properly.

**Q: Is it possible to list explicit mass payment histories filtering natively across accounts?**
This particular structural node maps explicit order manipulation limits. Operations resolving broad search queries or complex un-bounded transaction logs aren't exposed natively in this immediate abstraction scope for precise object handling.

**Q: Which parameter natively identifies bounds when generating refunds?**
Proper financial refunds are mapped utilizing strictly captured payment node structures. You must pass the specific Capture ID explicitly retrieved from logging the 'capture_order' action properly, not just initial limit bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paypal](https://vinkius.com/mcp/paypal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PayPal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paypal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PayPal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paypal": {
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
