# Donately MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donately-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage Donately fundraising and donor data using AI agents.

## Description
### What you can do
- Retrieve and list incoming donations.
- Manage and list your fundraising campaigns.
- Access donor information and contacts.
- Keep track of recurring subscriptions and peer-to-peer fundraisers.

### How it works
1. Subscribe to Donately.
2. Insert your API Token and Account ID.
3. Let the AI Agent fetch and manage your fundraising data.

### Who is this for?
Ideal for non-profits, NGOs, and fundraising teams who want to seamlessly query their Donately data through AI Agents.


## Available Tools (11)
- **get_donation**: Get details of a specific donation
- **get_fundraiser**: Get details of a specific peer-to-peer fundraiser
- **get_person**: Get details of a specific person (donor)
- **get_subscription**: Get details of a specific recurring donation (subscription)
- **list_campaigns**: Campaigns are the primary way to organize fundraising efforts.

List campaigns for the Donately account
- **list_donations**: Useful to track incoming contributions and donor activities. Supports pagination and filtering.

List donations for the Donately account
- **list_fundraisers**: List peer-to-peer fundraisers for the Donately account
- **list_people**: List people (donors/contacts) for the Donately account
- **list_subscriptions**: List recurring donations (subscriptions) for the Donately account
- **create_donation**: Create a new donation
- **get_campaign**: Get details of a specific campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donately** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent donations from Donately."

**🤖 AI Agent:**
> Here are your most recent donations...

---

**👤 You:**
> "Find details about a specific campaign."

**🤖 AI Agent:**
> I found the following details for your campaign...

---

**👤 You:**
> "Retrieve a list of our recurring subscriptions."

**🤖 AI Agent:**
> Here is the list of active recurring subscriptions...


## ❓ FAQ

**Q: Does the AI agent process payments directly?**
No, the AI agent retrieves and manages data from your Donately account, it does not act as a payment gateway itself.

**Q: Can the AI agent create new fundraising campaigns?**
Currently, the agent can list and retrieve information about existing campaigns, but campaign creation should be done in the Donately dashboard.

**Q: Is donor data safe with the AI agent?**
Yes, the agent only accesses the data necessary to answer your prompts and does not store personal donor information permanently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donately-alternative](https://vinkius.com/mcp/donately-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Donately** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donately-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Donately** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donately-alternative": {
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
