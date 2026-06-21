# RateUpdate MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rateupdate)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rateupdate-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rateupdate-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage hotel rates and availability across OTAs and booking channels with centralized distribution and pricing intelligence.

## Description
Connect your **RateUpdate** account to any AI agent and monitor mortgage rates through natural conversation.

### What you can do

- **Rate Monitoring** — View current rates and inspect individual rate details
- **Program Analysis** — List loan programs and review eligibility requirements
- **Rate Trends** — Track historical rate movements over custom periods
- **Lender Comparison** — Compare rates across lenders for any program
- **Alert Management** — View configured rate change alerts
- **Health Check** — Verify API connectivity


## Available Tools
- **check_rateupdate_status**: Verify API connectivity
- **compare_rates**: Compare rates by program
- **get_lender**: Get lender details
- **get_program**: Get program details
- **get_rate**: Get rate details
- **get_trends**: Get rate trends
- **list_alerts**: List rate alerts
- **list_lenders**: List lenders
- **list_programs**: List loan programs
- **list_rates**: List current mortgage rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RateUpdate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me current mortgage rates."

**🤖 AI Agent:**
> Here are 12 current rates. The best 30-year fixed is 6.25% from LenderA. The 15-year fixed starts at 5.75%. Would you like to compare rates for a specific program?

---

**👤 You:**
> "Compare rates for program prg_30yr_fixed."

**🤖 AI Agent:**
> Comparing 5 lenders for 30-Year Fixed: LenderA (6.25%), LenderB (6.375%), LenderC (6.50%). LenderA offers the lowest rate with 0.5 points.

---

**👤 You:**
> "Show rate trends for the last 30 days."

**🤖 AI Agent:**
> Over the last 30 days, the 30-year fixed rate dropped from 6.75% to 6.25% (-0.50%). The biggest daily drop was -0.125% on the 15th.


## Installation & Usage

To install and use the **RateUpdate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rateupdate](https://vinkius.com/mcp/rateupdate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
