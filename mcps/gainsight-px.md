# Gainsight PX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gainsight-px)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage product experience, track user behavior, and oversee engagements via AI agents with Gainsight PX.

## Description
Connect your **Gainsight PX** (Aptrinsic) account to any AI agent to automate your product analytics and in-app engagement workflows through the Model Context Protocol (MCP). Gainsight PX helps you drive product adoption by understanding user behavior and delivering personalized in-app experiences. This MCP server enables you to manage user and account profiles, track server-side custom events, and retrieve engagement metadata directly through natural conversation.

### Key Features

- **User & Account Orchestration** — Search and list users or accounts based on custom filters, and fetch detailed profile metadata instantly.
- **Profile Identification** — Programmatically create or update user and account profiles to ensure your identity mapping is always accurate.
- **Server-Side Event Tracking** — Log custom interaction events from your backend to enrich your product usage datasets without client-side code.
- **Feature Discovery** — Access and list all product features currently being tracked to understand your instrumentation coverage.
- **Engagement Insights** — Retrieve a list of active in-app guides, sliders, and surveys to monitor your communication strategy.
- **Multi-Region Support** — Seamlessly connect to your specific Gainsight PX data center (US or EU).
- **Real-time Synchronization** — Keep your product experience data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gainsight PX Region and API Key (found in Administration > Products)
3. Start managing your product analytics from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check user adoption metrics or verify if a specific feature is being tracked without manual dashboard navigation.
- **Growth Engineers** — automate the identification of new users or accounts via simple AI commands.
- **Customer Success Ops** — sync account metadata and track custom server-side events seamlessly.


## Available Tools (12)
- **verify_api_connection**: Check connection
- **get_account_details**: Get account metadata
- **get_my_identity**: Get account profile
- **get_user_details**: Get user metadata
- **identify_px_account**: Sync account profile
- **identify_px_user**: Sync user profile
- **list_px_accounts**: Query PX accounts
- **list_px_engagements**: List guides/surveys
- **list_product_features**: List tracked features
- **list_px_products**: List PX products
- **list_px_users**: Query PX users
- **track_server_event**: Log custom event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gainsight PX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all PX users who were last seen in the past 24 hours."

**🤖 AI Agent:**
> Querying users... I found 15 users active in the last 24 hours, including 'john.doe@example.com' and 'alice.smith@provider.com'. Would you like the full profile for any of them?

---

**👤 You:**
> "Identify a new account 'Globex Corp' with ID 'acc_98765'."

**🤖 AI Agent:**
> Account identified! I have successfully synchronized 'Globex Corp' (ID: acc_98765) to your Gainsight PX environment. Any future events for this ID will be attributed to this account.

---

**👤 You:**
> "Track a custom event 'Clicked Upgrade Button' for user 'user_123'."

**🤖 AI Agent:**
> Event tracked! The 'Clicked Upgrade Button' event has been successfully logged for user_123. This data will now appear in your product usage analytics.


## ❓ FAQ

**Q: How do I get an API Key for Gainsight PX?**
Log in to Gainsight PX, go to Administration > Products, select your product, and you will find the API Key in the product settings.

**Q: Which region should I select?**
Select 'US' if your account is hosted at api.aptrinsic.com, or 'EU' if it is hosted at api-eu.aptrinsic.com.

**Q: Can I identify new users through the agent?**
Yes! Use the 'identify_px_user' tool and provide a unique 'identifyId'. The agent will create or update the user profile in Gainsight PX instantly.

**Q: Does this server support tracking custom events?**
Yes, the 'track_server_event' tool allows you to log custom behavioral events for any identified user directly from your backend or chat interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gainsight-px](https://vinkius.com/mcp/gainsight-px)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gainsight PX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gainsight-px` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gainsight PX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gainsight-px": {
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
