# AwardWallet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/awardwallet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage loyalty points, travel rewards, and itineraries via AwardWallet — monitor your miles and trips directly via AI.

## Description
Connect your **AwardWallet** business account to any AI agent and track your loyalty points, frequent flyer miles, and travel itineraries through natural conversation.

### What you can do

- **Loyalty Tracking** — Monitor balances, expiration dates, and elite status across hundreds of frequent flyer and reward programs
- **Travel Timelines** — Access a unified view of past and upcoming trips, including flights, hotels, and car rentals
- **Itinerary Auditing** — Retrieve detailed metadata and confirmation details for trips shared by your connected users
- **User Access Control** — List and manage users who have authorized your business to access their travel and loyalty data

### How it works

1. Subscribe to this server
2. Enter your AwardWallet Business API Key
3. Start managing your travel rewards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Travelers** — instantly check point balances and trip details without searching through multiple emails
- **Travel Assistants** — coordinate itineraries and monitor expiration dates for team members from a single workspace
- **Operations Teams** — automate the auditing of corporate travel data and loyalty program status for employees


## Available Tools (9)
- **create_auth_url**: Generate an authorization URL for a user to link their AwardWallet account
- **get_account_check**: Verify AwardWallet Business API connection
- **get_account_details**: Get specific details for a loyalty account
- **get_account_history**: Retrieve historical activity for a specific loyalty account
- **get_user_accounts**: Retrieve loyalty account list for a specific user
- **get_user_itineraries**: Retrieve detailed itineraries for a specific user
- **get_user_timeline**: Retrieve the travel timeline for a specific user
- **list_connected_users**: List all AwardWallet users who have authorized your business account
- **list_loyalty_providers**: List all supported loyalty providers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AwardWallet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all connected users in my AwardWallet account."

**🤖 AI Agent:**
> I've retrieved your connected users. You currently have 3 users authorized: 'John Doe' (ID: 12345), 'Jane Smith' (ID: 67890), and 'Robert Brown'. Which user's rewards would you like to inspect?

---

**👤 You:**
> "Show me the loyalty accounts for user ID '12345'."

**🤖 AI Agent:**
> I've fetched the accounts for user 12345. They have 150,000 Delta SkyMiles (Gold Medallion) and 45,000 Marriott Bonvoy points. Note: The Marriott points expire in 3 months. Shall I check for more details?

---

**👤 You:**
> "Get the travel timeline for user '998877'."

**🤖 AI Agent:**
> Retrieving timeline... User 998877 has an upcoming flight to London (LHR) on June 15th and a hotel stay at 'The Savoy'. Their last trip was to Tokyo in February. Would you like the full itinerary for the London trip?


## ❓ FAQ

**Q: Can the AI automatically notify me about points that are expiring soon?**
Yes! You can ask the agent to check for upcoming point expirations across all connected users. It will use the `get_connected_user_accounts` tool to identify balances at risk and report them to you in seconds.

**Q: How do users authorize my business account to see their travel data?**
Simply ask the agent to run the `create_auth_url` tool. It will generate a unique authorization link that you can share with your users. Once they click and approve, their data becomes visible to your agent.

**Q: Is it possible to retrieve full flight confirmation details through the AI?**
Yes. The `get_itinerary` tool allows the agent to fetch complete trip details, including confirmation numbers, flight times, and hotel addresses for any shared trip.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awardwallet](https://vinkius.com/mcp/awardwallet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AwardWallet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `awardwallet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AwardWallet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "awardwallet": {
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
