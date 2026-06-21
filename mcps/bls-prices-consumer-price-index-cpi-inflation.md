# BLS Prices — Consumer Price Index (CPI) & Inflation MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-prices-consumer-price-index-cpi-inflation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bls-prices-consumer-price-index-cpi-inflation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bls-prices-consumer-price-index-cpi-inflation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the official source of US inflation data. Retrieve the Consumer Price Index (CPI-U), Producer Price Index (PPI), and precise historic metrics on the cost of living using the BLS v2 API.

## Description
Connect to the exact datasets used by the Federal Reserve and economists to measure US inflation. The Bureau of Labor Statistics Prices MCP gives your agent direct access to consumer and producer price fluctuations.

### What you can do
- **Consumer Price Index (CPI-U)** — Fetch changes in the prices paid by urban consumers for a market basket of consumer goods and services.
- **Producer Price Index (PPI)** — Track the average change over time in the selling prices received by domestic producers for their output.
- **Historical Metrics** — Query up to 20 years of consecutive inflation data instantly.

### How it works
1. Sign up for a free BLS Developer API Key
2. Provide the key in the settings
3. Ask your AI to calculate current inflation or track price changes since 2010.

### Who is this for?
- **Financial Analysts & Traders** — Build models off real macroeconomic signals
- **Economists & Researchers** — Direct access to historic US index data
- **Corporate Finance** — Adjust projections and budgets to accurate inflation curves


## Available Tools
- **get_cpi_inflation**: S. Consumer Price Index baseline. Identifies macroeconomic price shifts and consumer buying power anomalies.

Get Consumer Price Index (CPI-U) data for inflation tracking
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Prices — Consumer Price Index (CPI) & Inflation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the US inflation rate context in 2023?"

**🤖 AI Agent:**
> 📊 **Consumer Price Index (CPI) — 2023 Summary**

The CPI for All Urban Consumers (CPI-U) ended 2023 at **306.746** (December), up from **296.797** in December 2022. This represents an annual inflation rate of approximately **3.4%** for the year, significantly lower than the 6.5% rate seen in 2022, signaling an overall cooling of price increases.

---

**👤 You:**
> "How much did prices rise from January 2020 to January 2024?"

**🤖 AI Agent:**
> Based on the BLS CPI-U Index (CUUR0000SA0):

- **Jan 2020:** 257.971
- **Jan 2024:** 308.417

Prices rose by **19.55%** over this four-year period, driven primarily by post-pandemic supply chain issues and housing costs.

---

**👤 You:**
> "Analyze the Producer Price Index over the last two years."

**🤖 AI Agent:**
> 📉 **PPI Final Demand (PCUOMFGOMFG)**

Over the last 24 months, the Producer Price Index for Final Demand shifted dramatically from a peak year-over-year increase of 11.7% in mid-2022 to hovering near 1-2% entering 2024, signaling that input cost pressures on businesses have largely normalized.


## Installation & Usage

To install and use the **BLS Prices — Consumer Price Index (CPI) & Inflation** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-prices-consumer-price-index-cpi-inflation](https://vinkius.com/mcp/bls-prices-consumer-price-index-cpi-inflation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
