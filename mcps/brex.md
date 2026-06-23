# Brex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI to navigate your Brex suite. Spin up virtual cards, route new team members, and check daily cash allocations through natural chat.

## Description
The **Brex MCP Server** bridges standard large language models directly via the `platform.brexapis.com` to your startup's core spend engine. By delivering a single static User Token, you enable the most flexible financial assistant available.

### What you can do

- **Agile Employee Onboarding** — `brex_create_user` directly provisions employees with their associated hierarchical structure. Follow it up with `brex_create_card` to hand them digital spend capacity securely limited.
- **Accounting Snapshots** — You don't need to load the Brex dash to trace down runaway expenses. Trigger `brex_list_transactions` to pull highly contextualized raw CSV data into your AI workspace.
- **Accounts Payable Controls** — Draft and approve external entity vendors via `brex_create_vendor` and initiate routing payments `brex_pay_vendor` seamlessly, letting internal routing protocols map out the wires.

### How it works

1. In your Brex settings, you can generate an immediate `User Token` (typically starting with `user_token_`).
2. This token natively identifies you and limits AI actions safely within your existing managerial permissions level.
3. Drop this into your client credentials and authorize AI access.

### Who is this for?

- **Forward-Thinking CFOs / FinOps** — Handle your routine accounting actions strictly through language.
- **Startups Scaling** — Automatically loop AI agents to handle corporate card provisioning to cloud instances without manual checks.


## Available Tools (10)
- **brex_create_card**: Useful for giving employees isolated cards for SaaS subscriptions.

Issue a dynamic Virtual Corporate Card
- **brex_create_user**: You must provide a valid email, first name, and last name.

Invite a new employee / user to Brex
- **brex_create_vendor**: Create a Vendor in AP (Accounts Payable)
- **brex_get_balance**: Get main cash balance of the Brex Cash accounts
- **brex_list_budgets**: List budget programs assigned to teams
- **brex_list_cards**: List all issued cards across the company
- **brex_list_transactions**: Sweep historical Brex card and account transactions
- **brex_list_users**: List all users in the Brex company account
- **brex_list_vendors**: List saved Vendors inside Brex AP
- **brex_pay_vendor**: Orchestrate a vendor payment (Send Money)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Invite the new engineer 'John Carter' via email john@company.com into Brex. After you get his ID, spin him up a Virtual Card with a $1K limit immediately."

**🤖 AI Agent:**
> Double-tool chain complete! First, I invoked `brex_create_user` and instantiated John natively. Next, I utilized the Brex User UUID `usx_210` to successfully map and authorize a fresh Virtual Mastercard strictly capped at a 1000 limit.

---

**👤 You:**
> "Check the core cash settlement. How much Treasury base balance do we stand at? Extract only active Checking values."

**🤖 AI Agent:**
> According to the `cash/balances` API sweep, your primary operational checking environment sits at $145,210.00 USD securely settled by your local Brex vault integrations.

---

**👤 You:**
> "Pull all corporate expenses tracked over the past 30 days focusing entirely on our AWS hosting and digital footprints."

**🤖 AI Agent:**
> I performed a granular array analysis of over 50 transaction payloads returning from the last 30 intervals. Brex logs exactly three occurrences of AWS charges on the 'Engineering Budget'. Amounting to roughly $3,000 cumulatively.


## ❓ FAQ

**Q: Can the agent truly issue a real, functioning corporate card?**
Yes! The `brex_create_card` logic specifically maps to creating a virtual limit card. By default, it operates completely valid via Visa/Mastercard configurations matching Brex internals. The agent handles setting its name and tying it strictly to the user id.

**Q: What acts as the final authentication key for Brex?**
You only need a `User Token`. Brex explicitly supports personal workflow automation using `user_tokens` which perfectly mimic your permissions. It typically begins literally with the string `user_token_` followed by hashes.

**Q: Will vendor payments via AI require external 2FA from my side?**
To enforce safety in the integration, the `approval_type` parameter when sending vendor money defaults to `'MANUAL'`. This means the AI structures all the math, formatting, routing inputs perfectly but leaves the final 'Accept' button queued on your dashboard.

**Q: How can I see my user lists across Brex?**
Run a request on `brex_list_users`. The AI will natively stream the company's organizational tree mapping the emails to Brex UUIDs required for triggering corporate card injections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brex](https://vinkius.com/mcp/brex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brex": {
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
