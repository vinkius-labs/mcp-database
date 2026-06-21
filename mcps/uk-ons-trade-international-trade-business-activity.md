# UK ONS Trade — International Trade & Business Activity MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uk-ons-trade-international-trade-business-activity-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uk-ons-trade-international-trade-business-activity-mcp)
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


## Available Tools
- **get_trade**: Dataset: trade. Monthly data on UK trade in goods: imports, exports, trade balance by partner country and commodity. Non-seasonally adjusted. Values in £ million.

Get UK trade in goods data — country by commodity, imports and exports
- **get_business_counts**: Dataset: uk-business-by-enterprises-and-local-units. Source: Inter-Departmental Business Register (IDBR).

Get UK business counts by enterprises and local units, by industry and geography
- **get_traffic_activity**: Dataset: traffic-camera-activity. Used as a real-time indicator to understand economic activity and social change.

Get UK traffic camera activity — experimental economic indicator


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


## Installation & Usage

To install and use the **UK ONS Trade — International Trade & Business Activity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity](https://vinkius.com/mcp/uk-ons-trade-international-trade-business-activity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
