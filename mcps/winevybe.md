# Winevybe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/winevybe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Automate sommelier intelligence via Winevybe — search global wine catalogs, check vineyard ratings, and manage virtual cellars directly from any AI agent.

## Description
Connect your **Winevybe** developer account to any AI agent and take full control of sommelier intelligence and wine inventory tracking through natural conversation.

### What you can do

- **Sommelier Recommender** — Query for specific wine pairings and tasting notes magically linked behind intelligent algorithms
- **Inventory Management** — Read and append bottle quantities to persistent user cellars safely via automated workflows
- **Vintage Auditing** — Cross-reference a specific year to see if the region's climate conditions yielded good harvests
- **Pricing Comparisons** — Compare distinct bottles instantly to analyze pricing versus critical community reception
- **Vineyard Profiling** — Retrieve the underlying history and details of major worldwide producers and regions

### How it works

1. Subscribe to this server
2. Enter your Winevybe API Key
3. Start managing your wine library and tasting queries from Claude, Cursor, or any MCP-compatible client

No more manually searching through obscure tasting sites. Your AI acts as a dedicated sommelier tracking the exact market values and tasting notes of your private cellar.

### Who is this for?

- **Hospitality Managers** — instantly retrieve wine characteristics and pairing ideas without opening the Winevybe app
- **Private Collectors** — track the maturity of cellar inventory straight from a chat interface
- **Food Journalists & Creators** — gather highly specific regional scores to write reviews effortlessly


## Available Tools (10)
- **get_reviews**: Get community tasting reviews and ratings
- **get_user_cellar**: Examine the inventory of an authenticated users wine cellar
- **get_vintage_scores**: Get an overview of harvest qualities by year
- **get_wine_detail**: Get profound tasting notes and stats on a specific wine
- **get_winery_info**: Get profiles of specific vineyards and producers
- **search_wines**: Search the Winevybe database for specific bottles
- **add_wine_to_cellar**: Add a purchased bottle into a users virtual cellar tracker
- **compare_wines**: Generate a side-by-side contrast of two bottles
- **get_pairings**: Get food pairing recommendations for a specific wine
- **get_region_info**: Retrieve details about wine-making appellations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Winevybe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for details on the Screaming Eagle Cabernet Sauvignon."

**🤖 AI Agent:**
> I've fetched the profile details for 'Screaming Eagle Cabernet Sauvignon' (Wine ID: 39502). It is highly rated (98/100) and displays deep blackberry notes with incredibly refined tannins. Would you like to check pairing ideas?

---

**👤 You:**
> "Compare wine 4902 and wine 5910."

**🤖 AI Agent:**
> Running the comparison workflow... Wine 4902 is a Bordeaux Blend averaging $120, while wine 5910 is a Napa Valley Meritage averaging $145. Both rank highly on fruit structure, but 4902 offers a slightly higher rating relative to price.

---

**👤 You:**
> "Check my virtual cellar inventory."

**🤖 AI Agent:**
> Accessing your cellar (User ID: currentUser)... You currently hold 14 active bottles, spanning 3 primary varietals. Recent additions include the 'Louis Roederer Brut 2014'. Which section should we audit?


## ❓ FAQ

**Q: Can my AI automatically pull tasting notes and pairings out of a single bottle search?**
Yes! Use the `get_wine_detail` and `get_pairings` tools. Your agent will respond with complete metadata regarding aromas, tannin complexity, and best foods to match with the queried bottle.

**Q: How do I easily update the inventory inside my virtual cellar?**
Simply ask the agent to run the `add_wine_to_cellar` action providing the Wine ID and Quantity. It will modify your inventory database safely without manually clicking through menus.

**Q: Are there any destructive capabilities regarding regional scores or public metrics?**
No. The core set of tools dealing with global data limits itself strictly to querying records like `get_vintage_scores`. All write operations are firmly locked to your private user cellar.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/winevybe](https://vinkius.com/mcp/winevybe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Winevybe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `winevybe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Winevybe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "winevybe": {
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
