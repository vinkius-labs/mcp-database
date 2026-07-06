# Melo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/melo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

On-chain real estate intelligence via Melo — track properties, transactions, and market insights.

## Description
Connect your **Melo** account to any AI agent and take full control of your real estate intelligence and on-chain property data through natural conversation.

### What you can do

- **Property Management** — List all properties, search by address, and fetch detailed SKU metadata including on-chain IDs
- **Market Insights** — Access real-time AI-driven market trends and neighborhood analytics for specific locations
- **Transaction Monitoring** — Track property sales history and blockchain-native events securely
- **Listing Oversight** — Enumerate active property listings for sale or rent across different regions
- **Portfolio Auditing** — Retrieve historical data, price changes, and smart contract metadata for on-chain assets

### How it works

1. Subscribe to this server
2. Enter your Melo API Key
3. Start managing your real estate data from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_property**: Get details for a specific property
- **get_property_history**: Get historical data for a property
- **list_active_listings**: List all active property listings
- **list_property_collections**: List curated property collections
- **list_neighborhoods**: List neighborhoods in a city
- **list_properties**: List real estate properties
- **list_transactions**: List real estate transactions
- **search_properties**: Search properties by term
- **get_market_insights**: Get real estate market insights
- **get_onchain_metadata**: Get on-chain metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Melo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active properties in Austin, TX."

**🤖 AI Agent:**
> Retrieving properties... I found 5 active listings in Austin, including '123 Main St' ($450k) and '456 Oak Ave' ($620k).

---

**👤 You:**
> "Show market insights for Miami."

**🤖 AI Agent:**
> Querying insights... Miami is currently seeing a 5% increase in property values with high demand in the Brickell neighborhood.

---

**👤 You:**
> "Get transaction history for property ID 987."

**🤖 AI Agent:**
> Fetching history... Property 987 has 3 recorded transactions, the most recent being a sale for 150 ETH in 2023.


## ❓ FAQ

**Q: How do I find my Melo API Key?**
Log in to Melo, go to your Dashboard settings, and look for the API section to generate or copy your key.

**Q: What is 'on-chain' property data?**
This refers to real estate information recorded on a blockchain, providing a transparent and immutable history of ownership and events.

**Q: Is my real estate data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/melo](https://vinkius.com/mcp/melo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Melo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `melo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Melo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "melo": {
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
