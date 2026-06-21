# Gigs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gigs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage mobile subscriptions, track data usage, and oversee eSIMs via AI agents with Gigs.

## Description
Connect your **Gigs** telecom-as-a-service account to any AI agent to automate your mobile connectivity workflows through the Model Context Protocol (MCP). Gigs abstracts the complexity of global carriers into a unified API, allowing you to manage mobile plans and SIMs with ease. This MCP server enables you to retrieve connectivity plans, manage subscriber profiles (users), and track real-time data consumption directly through natural conversation.

### Key Features

- **Subscription Orchestration** — List all active and inactive mobile subscriptions, retrieve detailed configuration metadata, and create new subscriptions instantly.
- **Real-time Usage Tracking** — Retrieve up-to-the-minute consumption data (data, talk, text) for any subscription to monitor user behavior.
- **User Management** — Register new telecom users and manage their profiles programmatically from your chat interface.
- **Plan Discovery** — Access a comprehensive catalog of voice and data plans available in 200+ countries.
- **SIM Inventory Oversight** — List and retrieve metadata for both eSIMs and physical SIM cards.
- **Project Analytics** — Access high-level metadata for your connected Gigs projects to verify settings and connectivity.
- **Real-time Synchronization** — Keep your telecom operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gigs Project API Key (found in Dashboard > Settings > API Keys)
3. Start managing your mobile connectivity from Claude, Cursor, or any MCP client

### Who is this for?

- **Fintech & Ops Teams** — quickly check a customer's data usage or verify subscription status without manual portal navigation.
- **Product Managers** — get a real-time overview of available mobile plans and regional pricing via simple AI commands.
- **Customer Support** — verify eSIM activation status and troubleshoot connectivity issues seamlessly.


## Available Tools (12)
- **verify_api_connection**: Check connection
- **create_mobile_subscription**: Start new plan
- **create_telecom_user**: Add new user
- **get_account_details**: Get account identity
- **get_plan_details**: Get plan metadata
- **get_subscription_details**: Get subscription metadata
- **get_subscription_usage**: Check data usage
- **list_connectivity_plans**: List mobile plans
- **list_telecom_projects**: List Gigs projects
- **list_connectivity_sims**: List SIM cards
- **list_mobile_subscriptions**: List all subscriptions
- **list_connectivity_users**: List telecom users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gigs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available mobile data plans in the catalog."

**🤖 AI Agent:**
> Retrieving plans... I found 15 available plans, including 'USA 5GB Data' (ID: plan_123) and 'Global Unlimited Talk & Text'. Would you like the pricing details for any of them?

---

**👤 You:**
> "How much data has user 'sub_98765' used this month?"

**🤖 AI Agent:**
> Checking usage... User sub_98765 has consumed 2.4 GB of their 5 GB data cap. They have also used 45 minutes of talk time and sent 12 text messages.

---

**👤 You:**
> "Create a new subscription for 'john@example.com' using plan 'plan_abc'."

**🤖 AI Agent:**
> Subscription created! I have successfully attached plan plan_abc to user john@example.com. The new Subscription ID is 'sub_555' and the eSIM is ready for activation.


## ❓ FAQ

**Q: How do I get an API Key for Gigs?**
Log in to your Gigs Dashboard, navigate to Settings > API Keys, and you can generate a new Project API Key there.

**Q: Can I see real-time data consumption?**
Yes! Use the 'get_subscription_usage' tool with a Subscription ID to retrieve the current data, talk, and text consumption for that specific user.

**Q: Does Gigs support both eSIM and physical SIM cards?**
Yes, Gigs provides unified management for both digital eSIMs and physical hardware. You can list your inventory using the 'list_connectivity_sims' tool.

**Q: How do I activate a new subscription?**
First, create a user with 'create_telecom_user', then use the 'create_mobile_subscription' tool to attach a specific plan ID to that user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gigs](https://vinkius.com/mcp/gigs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gigs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gigs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gigs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gigs": {
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
