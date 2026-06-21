# BLS JOLTS — Job Openings, Quits & Turnover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-jolts-job-openings-quits-turnover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bls-jolts-job-openings-quits-turnover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bls-jolts-job-openings-quits-turnover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Deep-dive into the 'Great Resignation' and labor tightness with the US Job Openings and Labor Turnover Survey (JOLTS). Track hires, fires, and voluntary quits.

## Description
Understand labor supply and demand dynamics utilizing the exact JOLTS (Job Openings and Labor Turnover Survey) API.

### Core Metrics Included
- **Quits Level** (The 'Great Resignation' index)
- **Hires Level**
- **Layoffs & Discharges**
- **Job Openings**

### Who is this for?
- Macro-Traders scanning for labor market cracks before the stock market opens.
- Economists measuring the 'quits' rate to forecast wages.


## Available Tools
- **get_jolts_data**: Critical for determining the Great Resignation impacts.

Get Job Openings (JOLTS) national metrics
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS JOLTS — Job Openings, Quits & Turnover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest reading on total job openings?"

**🤖 AI Agent:**
> JOLTS shows 8.79 million open jobs natively available across the U.S., trending downward from the post-pandemic high of 12.1 million.

---

**👤 You:**
> "Compare Quits vs Layoffs over the last quarter."

**🤖 AI Agent:**
> Quits maintained a rate of 2.2% (approx 3.4M workers) while overall Layoffs stood at incredibly low historic bounds of 1.0% (1.5M workers), signaling strong worker conviction.

---

**👤 You:**
> "Summarize the turnover for Information / Tech sectors."

**🤖 AI Agent:**
> The Tech/Information sector observed an uptick in layoffs combined with a dramatic slowdown in hires, showing net-zero payroll generation in the short-term.


## Installation & Usage

To install and use the **BLS JOLTS — Job Openings, Quits & Turnover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-jolts-job-openings-quits-turnover](https://vinkius.com/mcp/bls-jolts-job-openings-quits-turnover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
