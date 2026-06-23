# Authorize.net MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/authorizenet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process cards, manage refunds, capture holds, and inspect settled transactions on Authorize.net directly from your AI agent.

## Description
Connect your **Authorize.net** merchant gateway to any AI agent to power conversational commerce. Command precise payment logic, track settlements, and manage Customer Information Manager (CIM) profiles effortlessly.

### What you can do

- **Payment Processing** — Run strict "Auth & Capture" to process real funds instantly, or perform "Auth Only" to hold funds legitimately before shipping
- **Refunds & Voids** — Initiate refunds on previously settled transactions or Void anomalies residing in your pending batches cleanly
- **Vault & CIM Profiles** — Securely construct isolated Customer Information Profiles linking sensitive card data without exposing raw PANs to unencrypted bounds
- **Auditing & Settlements** — Query distinct details of a single transaction ID or map an overarching list of today's unsettled nightly batch runs

### How it works

1. Subscribe to this secure MCP Server
2. Add your Authorize.net Login ID, Transaction Key, and Environment mapping
3. Engage directly with Authorize.net's API via Claude, Cursor, or any compatible AI client

Your AI agent eliminates the clunky Merchant Interface, managing daily financial anomalies in pure dialogue.

### Who is this for?

- **E-Commerce Managers** — seamlessly execute post-return refunds dynamically on the fly
- **Sales Engineers** — verify exactly why a card was declined (AVS or CVV logic flaws) natively
- **Financial Ops** — track unresolved unsettled holds systematically prior to batch processing


## Available Tools (10)
- **add_payment_profile**: Add a payment card to an existing CIM customer profile
- **auth_capture_transaction**: Perform an Authorize.net authorization and capture transaction
- **auth_only_transaction**: Place a temporary authorization hold on a credit card
- **prior_auth_capture**: Capture a previously authorized transaction hold
- **create_customer_profile**: net before securely attaching payment cards.

Create a new Customer Information Manager (CIM) profile
- **get_customer_profile**: Retrieve details of a Customer Information Manager (CIM) profile
- **get_transaction_details**: Get comprehensive details of a specific gateway transaction
- **get_unsettled_transactions**: List all unsettled transactions pending batch closure
- **refund_transaction**: You must pass the original transaction ID, the refund amount, and the original masked or raw PAN and expiration.

Refund an already settled Authorize.net transaction
- **void_transaction**: Void an unsettled Authorize.net transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Authorize.net** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unsettled transactions from the daily batch flow."

**🤖 AI Agent:**
> Interrogating unsettled items... 6 transactions are currently floating awaiting nightly batching. Notably, ID `6001293` for `104.50 USD` and ID `6001294` pending `20.00 USD`. Will you be voiding any of these anomalies today?

---

**👤 You:**
> "Get detailed properties masking transaction ID 719200."

**🤖 AI Agent:**
> Querying gateway depths... Target `719200` represents an Auth Capture worth `25.99 USD`. Status stands decisively at Settled Successfully. AVS mapped completely matching addresses while CVV verification yielded an unremarked clean 'Match'. All clear here unconditionally without discrepancies or concerns found.

---

**👤 You:**
> "Execute an immediate void on transaction 91230 as unauthorized."

**🤖 AI Agent:**
> Initiating Void payload to Authorize.net... Success achieved. Transaction `91230` has been stripped and obliterated successfully avoiding batch capture entirely. The associated card strings will organically restore the missing limits swiftly within general issuer intervals natively.


## ❓ FAQ

**Q: Can my AI safely create standard CIM profiles?**
Yes. The agent utilizes Authorize.net's API structure strictly intended for PCI-compliant scenarios. It successfully tokens the user emails converting them into shielded unique underlying node endpoints (Profile ID). Subsequent commands elegantly pin payment PAN inputs strictly onto that boundary.

**Q: Why would I use "Auth Only" instead of "Auth Capture"?**
An "Auth Only" is essential when shipping physical goods that aren't instantly ready. It guarantees the user's funds exist and freezes them for up to 30 days without legally withdrawing the cash. Once the shipment processes, your AI issues a Prior Auth Capture logically finishing the monetary path.

**Q: Is it possible to completely void transactions instead of waiting for a settlement?**
Yes. Authorize.net supports a strict "Void" capability on unsettled transactions. The AI can cancel a transaction if asked quickly within the same business day, preventing the funds from ever being captured in the overnight batch—saving you settlement and processing fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authorizenet](https://vinkius.com/mcp/authorizenet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Authorize.net** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `authorizenet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Authorize.net** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "authorizenet": {
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
