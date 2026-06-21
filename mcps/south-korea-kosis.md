# South Korea KOSIS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/south-korea-kosis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/south-korea-kosis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/south-korea-kosis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query official South Korean government statistics — demographics, GDP, trade, technology, and industry — from the KOSIS national database.

## Description
The **South Korea KOSIS MCP Server** connects your AI agent to the Korean Statistical Information Service — the official data portal for the world's 12th-largest economy and a global powerhouse in semiconductors, automotive, and electronics.

### Core Capabilities

- **Table Search** — Discover statistical tables across all Korean government agencies by keyword. Covers the full spectrum from demographics and national accounts to semiconductor production and trade flows.
- **Data Retrieval** — Pull raw numerical data from any KOSIS table, organized by classification and time period with full unit annotations.
- **Period Filtering** — Narrow results to specific time ranges using start/end period parameters.

Free API key required (instant registration at kosis.kr). South Korea publishes highly granular data covering semiconductor exports, technology adoption, and manufacturing output — intelligence that is critical for supply chain analysis and technology market research.


## Available Tools
- **get_korea_stats_data**: Requires orgId and tableId from search_korea_statistics. Optionally filter by time period (YYYYMM or YYYY format).

Retrieve statistical data from a specific KOSIS table in South Korea
- **search_korea_statistics**: Returns table IDs, organization IDs, and table names. Use returned orgId and tableId with get_korea_stats_data to retrieve numbers. Common topics: population, GDP, semiconductor exports, technology, employment, trade, education, housing.

Search for statistical tables in the South Korean KOSIS national database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **South Korea KOSIS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are South Korea's semiconductor export figures for the last 3 years?"

**🤖 AI Agent:**
> I've queried KOSIS for semiconductor trade data. South Korea's semiconductor exports reached approximately $132 billion in 2023, rebounding strongly from the $101 billion dip in 2022. Samsung and SK Hynix continue to dominate global memory chip production, driving the recovery.

---

**👤 You:**
> "What is South Korea's current population growth rate?"

**🤖 AI Agent:**
> Based on the latest KOSIS demographic data, South Korea's population growth rate is currently negative, standing at approximately -0.1%, driven by a record low total fertility rate.

---

**👤 You:**
> "Show me the employment statistics for the manufacturing sector this quarter."

**🤖 AI Agent:**
> According to KOSIS labor force survey data, employment in the manufacturing sector for Q3 reached 4.45 million workers, representing a 1.2% year-over-year growth, largely supported by automotive exports.


## Installation & Usage

To install and use the **South Korea KOSIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/south-korea-kosis](https://vinkius.com/mcp/south-korea-kosis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
