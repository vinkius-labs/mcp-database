# BLS Wages — OEWS Occupational Employment MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-wages-oews-occupational-employment)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bls-wages-oews-occupational-employment-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bls-wages-oews-occupational-employment-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

The holy grail of HR data. Use Occupational Employment and Wage Statistics (OEWS) to extract exact median earnings broken down by detailed professions and states.

## Description
If you need to know exactly how much a 'registered nurse in Texas' or a 'software engineer in Illinois' earns, OEWS is your required dataset.

### What you can find
- **Median / Average Pay** — Discover true wage distributions percentiles.
- **Occupation Codes** — Maps hundreds of distinct professions.
- **State Comparisons** — Compare geographic locations for job offers.


## Available Tools
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Wages — OEWS Occupational Employment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the median salary for Software Developers in Texas versus California?"

**🤖 AI Agent:**
> Software Developers in California enjoy a median wage upward of $150,000, whereas the median in Texas is closer to $120,000.

---

**👤 You:**
> "Tell me the hourly wage differences for Registered Nurses nationally."

**🤖 AI Agent:**
> Registered Nurses nationally see an average hourly boundary of roughly $42.80, with highs well past $60 in coastal markets.

---

**👤 You:**
> "Compare top 90th percentile to bottom 10th for Accountants."

**🤖 AI Agent:**
> Entry-level (10th percentile) Accountants run near $48,000 yearly, standing in stark contrast to the top executive counterparts (90th percentile) pushing toward $135,000+.


## Installation & Usage

To install and use the **BLS Wages — OEWS Occupational Employment** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-wages-oews-occupational-employment](https://vinkius.com/mcp/bls-wages-oews-occupational-employment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
