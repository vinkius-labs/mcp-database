# Giftbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giftbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Order, send, and track digital gift cards and rewards via AI agents with Giftbit.

## Description
Connect your **Giftbit** account to any AI agent to automate the delivery and tracking of digital rewards through the Model Context Protocol (MCP). Giftbit is a powerful rewards platform that lets you send digital gift cards to customers, employees, or research participants. This MCP server enables you to order new rewards, retrieve available brands, and track gift redemption statuses directly through natural conversation.

### Key Features

- **Reward Campaigns** — Programmatically create new campaigns to send digital rewards via Giftbit's customizable email delivery system.
- **Direct & Embedded Links** — Generate raw reward URLs (direct links) or embeddable links to distribute rewards through your own app or SMS.
- **Brand Discovery** — List all available reward brands, filter by region, and check allowed price ranges and metadata.
- **Redemption Tracking** — Retrieve detailed status updates for individual gifts to see if recipients have opened or claimed their rewards.
- **Campaign Oversight** — List past campaigns and fetch their completion and delivery statuses.
- **Environment Control** — Switch between the Giftbit 'testbed' (sandbox) for safe testing and 'production' for real transactions.
- **Real-time Synchronization** — Keep your reward fulfillment operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Giftbit API Token (from the developer portal)
3. Start managing your rewards from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing & CX Teams** — quickly check if a customer has claimed their apology gift or send a new reward instantly without manual dashboard navigation.
- **HR & Operations** — automate employee recognition campaigns via simple AI commands.
- **Product Teams** — generate embedded reward links on-the-fly for user research incentives.


## Available Tools
- **verify_api_connection**: Verify connectivity
- **order_email_rewards**: Send rewards via email
- **create_reward_links**: Generate direct links
- **create_embedded_links**: Generate embedded rewards
- **get_brand_details**: Get brand metadata
- **get_campaign_status**: Check campaign details
- **get_gift_status**: Check gift details
- **list_reward_brands**: List available brands
- **list_reward_campaigns**: List sent campaigns
- **list_gift_records**: List sent gifts
- **list_delivery_regions**: List regions
- **check_api_health**: Check API health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Giftbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List available reward brands in the US region."

**🤖 AI Agent:**
> Retrieving brands... I found several options for the US, including 'Amazon', 'Starbucks', and 'Target'. Would you like the minimum/maximum allowed prices for any of them?

---

**👤 You:**
> "Check the status of gift 'uuid-12345'."

**🤖 AI Agent:**
> Fetching gift status... The gift was 'DELIVERED' yesterday, and the redemption status is currently 'CLAIMED'. The recipient selected a Starbucks card.

---

**👤 You:**
> "Generate 3 direct links for a $10.00 Amazon card."

**🤖 AI Agent:**
> Links generated! I have successfully created 3 direct links for a $10.00 Amazon card (1000 cents). The short URLs are: [Link 1], [Link 2], and [Link 3].


## ❓ FAQ

**Q: How do I get an API Token for Giftbit?**
Log in to the Giftbit Developer Portal, navigate to the API settings, and you can generate an API Token for either your Testbed or Production account.

**Q: Can I test the integration without sending real money?**
Yes! Giftbit provides a fully functional 'testbed' environment. Simply set the 'Environment' credential to 'testbed' and provide your test API token.

**Q: What is the difference between direct links and embedded links?**
Direct links send the user to a standalone claim page. Embedded links are designed to be displayed directly within an iframe in your own application.

**Q: How do I specify the reward value?**
Giftbit handles all pricing in cents. To send a $5.00 reward, you must provide '500' as the price_in_cents parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giftbit](https://vinkius.com/mcp/giftbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Giftbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `giftbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Giftbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "giftbit": {
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
