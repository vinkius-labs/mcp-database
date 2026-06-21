# Lit Protocol (Decentralized Access Control) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lit-protocol-decentralized-access-control)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage decentralized access control, Programmable Key Pairs (PKPs), and execute immutable Lit Actions within TEEs directly from your AI agent.

## Description
Connect to **Lit Protocol** to orchestrate decentralized identity and access control. This server allows your AI to manage Programmable Key Pairs (PKPs), organize them into groups, and execute secure Lit Actions.

### What you can do

- **Account Management** — Create accounts, verify existence, and manage scoped usage API keys for secure day-to-day operations.
- **Programmable Key Pairs (PKP)** — Generate and list decentralized wallets (PKPs) owned by your account to act as distributed identities.
- **Access Control Groups** — Create groups, add/remove PKPs, and manage permissions for complex decentralized access schemas.
- **Lit Actions** — Register and execute immutable JavaScript programs inside Trusted Execution Environments (TEEs) using IPFS CIDs or inline code.
- **Security & Permissions** — Update usage key scopes and manage action-to-group mappings dynamically to ensure granular control.

### How it works

1. Subscribe to this server
2. Enter your Lit Protocol API Key
3. Start managing decentralized keys and executing secure actions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — automate the management of PKPs and Lit Actions without leaving your development environment.
- **Security Engineers** — audit access control groups and manage usage keys through natural language queries.
- **dApp Builders** — quickly test and execute Lit Actions in TEEs to verify decentralized logic.


## Available Tools
- **add_action_to_group**: Add an IPFS CID to a group
- **add_action**: Register a standalone action (name + CID)
- **add_group**: Create a new group
- **add_pkp_to_group**: Add a PKP to a specific group
- **add_usage_api_key**: Create a scoped usage key
- **check_account_exists**: Verify if an account exists for the provided API key
- **confirm_payment**: Finalize credit top-up after payment
- **create_account**: Create a new Lit account
- **create_payment_intent**: Create a Stripe PaymentIntent (min $5.00)
- **create_wallet**: Request a new PKP for the account
- **execute_lit_action**: Provide either code or ipfs_id.

Execute a Lit Action
- **get_billing_balance**: Check credit balance
- **list_actions**: List registered actions
- **list_api_keys**: List usage keys (metadata only)
- **list_groups**: List all groups
- **list_wallets**: List all PKPs owned by the account
- **remove_group**: Delete a group
- **remove_pkp_from_group**: Remove a PKP from a group
- **remove_usage_api_key**: Delete a usage key
- **update_usage_api_key**: Update permissions for a usage key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lit Protocol (Decentralized Access Control)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my PKP wallets and their addresses."

**🤖 AI Agent:**
> I've retrieved your PKPs. You have 2 active wallets: PKP #1 (Address: 0x123...) and PKP #2 (Address: 0x456...). Would you like to manage permissions for any of them?

---

**👤 You:**
> "Execute this Lit Action code to sign a message: 'console.log("signing...");'"

**🤖 AI Agent:**
> Executing the Lit Action in a TEE... The execution was successful. The output logs show 'signing...' and the operation completed securely. Do you need the execution receipt?

---

**👤 You:**
> "Create a new access group named 'Beta Testers'."

**🤖 AI Agent:**
> Group 'Beta Testers' has been created successfully with ID 'group_987'. You can now add PKPs to this group using the `add_pkp_to_group` tool.


## ❓ FAQ

**Q: Can I execute custom JavaScript code securely within a TEE?**
Yes! Use the `execute_lit_action` tool. You can provide either inline JavaScript code or an IPFS CID to run immutable programs inside Lit's Trusted Execution Environments.

**Q: How do I see all the decentralized wallets (PKPs) associated with my account?**
Simply use the `list_wallets` tool. It will return all Programmable Key Pairs (PKPs) owned by your account, including their IDs and addresses.

**Q: Is it possible to organize access control by grouping different identities?**
Absolutely. You can use `add_group` to create a new group and then `add_pkp_to_group` to manage which decentralized identities belong to that specific access schema.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lit-protocol-decentralized-access-control](https://vinkius.com/mcp/lit-protocol-decentralized-access-control)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lit Protocol (Decentralized Access Control)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lit-protocol-decentralized-access-control` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lit Protocol (Decentralized Access Control)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lit-protocol-decentralized-access-control": {
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
