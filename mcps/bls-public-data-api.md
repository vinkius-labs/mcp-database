# BLS Public Data API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-public-data-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bls-public-data-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bls-public-data-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access labor statistics — audit economic series and trends via AI.

## Description
Empower your AI agent to orchestrate your entire economic research and labor auditing workflow with the **BLS Public Data API**, the authoritative source for United States Bureau of Labor Statistics data. By connecting the BLS API to your agent, you transform complex macroeconomic searches into a natural conversation. Your agent can instantly retrieve historical time series data, audit employment trends, and query specific series IDs without you ever touching a government portal. Whether you are conducting market research or managing regional economic constraints, your agent acts as a real-time data analyst, ensuring your intelligence is always verified and precise.

### What you can do

- **Series Auditing** — Retrieve high-resolution time series data for thousands of BLS identifiers and maintain a clear view of economic changes.
- **Trend Oversight** — Audit historical labor statistics to understand the longitudinal distribution of economic scale instantly.
- **Economic Discovery** — Query specific series IDs like the Consumer Price Index (CPI) to identify relevant fiscal markers for your research.
- **Metadata Intelligence** — Retrieve unique series identifiers and year-based metadata to assist in deep-dive data classification.
- **Operational Monitoring** — Check API status to ensure your economic research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your BLS Registration Key
3. Start managing your economic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Policy Analysts** — monitor labor trends and retrieve official metadata straight from your workflow.
- **Researchers & Students** — verify economic data and audit series patterns without manual searching.
- **Financial Journalists** — perform rapid audits of inflation markers and identify relevant economic patterns through natural language.
- **Operations Leads** — automate statistical data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_api_status**: Check if the BLS Public Data service is operational
- **get_bls_timeseries_data**: Provide series IDs as a comma-separated string (e.g., "CUUR0000SA0,LNS14000000").

Get historical data for specific BLS series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Public Data API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get Consumer Price Index (CPI) data for the last 5 years using BLS."

**🤖 AI Agent:**
> I've retrieved the CPI data (Series ID: CUUR0000SA0)! The latest values show an inflation trend of [Value] for [Year]. I can provide the full historical breakdown or the monthly percent change metadata for you.

---

**👤 You:**
> "Show employment statistics for series 'LNS14000000' (Unemployment Rate)."

**🤖 AI Agent:**
> I've identified the unemployment rate series! The recent data points indicate a rate of [Value]% as of [Period]. I can assist you with an audit of other related employment markers if you'd like.

---

**👤 You:**
> "Compare data for series 'WPUFD4' and 'WPUFD491' from 2020 to 2023."

**🤖 AI Agent:**
> I've retrieved the data for both series! There are notable distributions in values between the primary and sub-category markers from 2020 to 2023. I can provide the comparative metadata breakdown to assist in your fiscal research.


## Installation & Usage

To install and use the **BLS Public Data API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-public-data-api](https://vinkius.com/mcp/bls-public-data-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
