# UK ONS Trade — International Trade & Business Activity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

UK trade and business statistics: trade in goods by country and commodity (imports, exports, balance), business counts by industry and geography from the IDBR register, and experimental traffic camera activity indicators from the ONS.

## Description
UK trade and business data.

### What you can do
- **Trade** — Imports/exports by country and commodity
- **Business Counts** — Enterprises by industry and region
- **Traffic Activity** — Experimental real-time indicator


## Available Tools (3)
- **get_trade**: Dataset: trade. Monthly data on UK trade in goods: imports, exports, trade balance by partner country and commodity. Non-seasonally adjusted. Values in £ million.

Get UK trade in goods data — country by commodity, imports and exports
- **get_traffic_activity**: Dataset: traffic-camera-activity. Used as a real-time indicator to understand economic activity and social change.

Get UK traffic camera activity — experimental economic indicator
- **get_business_counts**: Dataset: uk-business-by-enterprises-and-local-units. Source: Inter-Departmental Business Register (IDBR).

Get UK business counts by enterprises and local units, by industry and geography


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK ONS Trade — International Trade & Business Activity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are UK trade figures with the EU?"

**🤖 AI Agent:**
> 📊 **UK Trade with EU (Latest)**

Exports to EU: £14.2 billion
Imports from EU: £22.8 billion
Trade deficit: -£8.6 billion

Top exports: machinery, vehicles, chemicals
Top imports: vehicles, food, machinery

Source: ONS, trade dataset

---

**👤 You:**
> "What were the UK's top exports to the US last year?"

**🤖 AI Agent:**
> According to ONS trade commodity datasets, the UK's top exports to the United States include medicinal and pharmaceutical products, mechanical power generators, and cars/vehicles.

---

**👤 You:**
> "How many active IT businesses are registered in London?"

**🤖 AI Agent:**
> Based on the Inter-Departmental Business Register (IDBR) counts, there are approximately 58,000 active enterprises classified within the Information and Communication sector in the London region.


## ❓ FAQ

**Q: What is the IDBR?**
The Inter-Departmental Business Register (IDBR) is a comprehensive list of UK businesses used for all government statistical surveys. It covers 2.7 million+ live enterprises across all sectors.

**Q: Does this cover both goods and services?**
Currently, the primary datasets focus extensively on the trade in goods by commodity and country. Trade in services data is also available but categorized separately in larger macroeconomic releases.

**Q: What kind of traffic activity data is available?**
The ONS provides experimental real-time indicators compiled from traffic camera activity, which measure vehicle counts and traffic movement as a proxy for economic and supply chain activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity](https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK ONS Trade — International Trade & Business Activity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-ons-trade-international-trade-business-activity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK ONS Trade — International Trade & Business Activity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-ons-trade-international-trade-business-activity": {
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
