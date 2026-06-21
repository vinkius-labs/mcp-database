# Eurostat Trade — EU International Commerce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-trade-eu-international-commerce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eurostat-trade-eu-international-commerce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eurostat-trade-eu-international-commerce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

EU international trade data: imports and exports by partner country and product classification (SITC), industrial production index, retail trade volume, and services sector statistics for all 27 EU member states.

## Description
Track EU trade flows and industrial activity across all 27 member states.

### What you can do
- **Trade Balance** — EU imports/exports by partner country
- **Trade by Product** — SITC product classification
- **Industrial Production** — Monthly index by sector (NACE)
- **Retail Trade** — Volume index as consumer spending proxy
- **Generic Query** — Any trade/industry dataset


## Available Tools
- **get_trade_balance**: Dataset: ext_lt_maineu. Key partners: US, CN, UK, JP, CH.

Get EU international trade balance by partner country
- **get_trade_by_product**: Dataset: ext_st_eu27_2020sitc. Covers food, raw materials, fuels, chemicals, machinery, manufactured goods.

Get EU trade by product classification (SITC)
- **get_industrial_production**: Base year 2015=100. Breakdown by NACE sector. A leading indicator of economic activity.

Get EU industrial production index by country and sector
- **get_retail_trade**: Consumer spending proxy. Covers food, non-food, and online retail.

Get EU retail trade volume index
- **get_trade_dataset**: Common codes: ext_tec01, sts_inpr_m, sts_trtu_m, sbs_na_ind_r2.

Query any Eurostat trade/industry dataset by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eurostat Trade — EU International Commerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the EU trade balance with China?"

**🤖 AI Agent:**
> 🇨🇳 **EU-China Trade**

Exports to China: €230B
Imports from China: €512B
Trade deficit: -€282B

China is the EU's #1 source of imports and #3 export destination.
Top imports: electronics, machinery, textiles.
Top exports: vehicles, machinery, chemicals.

---

**👤 You:**
> "Show industrial production trends for Germany"

**🤖 AI Agent:**
> 🏭 **Germany — Industrial Production Index (2015=100)**

Latest: 94.2 (-5.8% below 2015)
12m trend: ↓ declining
Manufacturing: 92.1
Energy-intensive: 81.3 (severe decline)

German industry faces structural headwinds from high energy costs.

---

**👤 You:**
> "How is retail trade performing in the EU?"

**🤖 AI Agent:**
> 🛒 **EU Retail Trade Volume (2015=100)**

EU27: 108.3 (+2.1% YoY)
Online retail: +12% growth
Food: stable (+0.4%)
Non-food: +3.2%

E-commerce continues to drive overall retail growth.


## Installation & Usage

To install and use the **Eurostat Trade — EU International Commerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-trade-eu-international-commerce](https://vinkius.com/mcp/eurostat-trade-eu-international-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
