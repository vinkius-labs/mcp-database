# Ping++ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ping)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Bring unified payment intelligence to your AI with Ping++. Integrate WeChat, Alipay, and UnionPay through a single clean API interface.

## Description
Empower your Agent to seamlessly manage Chinese payment ecosystems with **Ping++**, the ultimate multi-channel payment aggregator. Connect to WeChat Pay, Alipay, UnionPay, and multiple other networks through a single, elegant interface, replacing complex point-to-point integrations.

### What you can do

- **Unified Charges** — Create and manage transactions across any supported payment channel
- **Refund Management** — Process and retrieve refunds across any network without learning specific gateway APIs
- **Customer Synchronization** — Create and track customer profiles and saved payment methods across platforms

### How it works

1. Subscribe to this server
2. Obtain your Secret API Key from your [Ping++ Developer Dashboard](https://dashboard.pingxx.com)
3. Inject the server into your LLM client and instantly manage multi-channel billing flows

### Who is this for?

- **E-Commerce Agents** — Automate refunds, track transaction states, and manage cross-channel payments seamlessly
- **Financial Operators** — Consolidate the management of WeChat and Alipay transactions without touching backend code
- **Developers in China** — Connect multiple SDK backends to a single MCP endpoint to rapid prototype monetization


## Available Tools
- **create_charge**: Requires the order_no, amount, app ID, channel, currency, subject, and body.

Create a new charge (payment request)
- **create_customer**: Create a new Customer
- **create_refund**: Create a refund for a specific charge
- **list_charges**: List existing charges
- **list_customers**: List existing Customers
- **retrieve_charge**: Retrieve the details of an existing charge
- **retrieve_customer**: Retrieve Customer details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ping++** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 successful charges for my Ping++ app."

**🤖 AI Agent:**
> Here are your last 5 incoming charges across all payment channels. Three originated from WeChat Pay (wx_lite) and two from Alipay. Total amount processing: 12500 CNY.

---

**👤 You:**
> "Create a new refund of 100 CNY for charge ID ch_xyz789."

**🤖 AI Agent:**
> I've successfully created the refund for charge `ch_xyz789` (Amount: 10000 cents). The status is currently marked as 'pending' with the downstream payment channel.

---

**👤 You:**
> "Show me the details for customer ID cus_12345."

**🤖 AI Agent:**
> Customer `cus_12345` was created on Oct 12. They have two saved payment methods bound, including one UnionPay source, and an empty balance.


## ❓ FAQ

**Q: Which API Key do I use?**
You must use your Secret Key (Live or Test mode). Do not use the Publishable Key as it lacks permission to perform backend actions across the Ping++ network.

**Q: How do payment channels differ?**
Each channel (e.g. `alipay_web`, `wx_pub`, `upacp`) corresponds to a specific environment (Web, WeChat Official Account, UnionPay App). Provide the appropriate channel string when creating a charge.

**Q: Does this handle RSA Signatures automatically?**
For core operations covered by the standard MCP, API keys are sufficient. Operations requiring dedicated RSA enterprise signing may need custom webhook verifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ping](https://vinkius.com/mcp/ping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ping++** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ping` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ping++** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ping": {
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
