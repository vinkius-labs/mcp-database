# DecileHub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/decilehub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/decilehub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/decilehub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Segment your customers by value and behavior with predictive analytics that reveal your most profitable audience segments.

## Description
Connect your **DecileHub** account to any AI agent and take full control of your venture capital and private equity fund operations through natural conversation.

### What you can do

- **Fund Management** — List all funds with AUM, strategy, and vintage year, and inspect individual fund details including commitments and portfolio allocation
- **Performance Analytics** — Retrieve IRR, TVPI, DPI, and benchmark comparisons for any fund
- **Portfolio Companies** — Browse all portfolio companies with valuations, fund allocations, and investment round history
- **Valuation Tracking** — Access historical valuation marks and unrealized value changes over time for each portfolio company
- **LP Management** — List limited partners with commitment amounts, distributions, and allocation profiles
- **Regulatory Compliance** — Browse and download regulatory filings and compliance reports

### How it works

1. Subscribe to this server
2. Enter your DecileHub API Token from Settings > API
3. Start managing your fund operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GP / Fund Managers** — query fund performance metrics, review portfolio company valuations, and check LP commitments without switching to the dashboard
- **Investor Relations** — pull LP profiles, commitment summaries, and distribution histories for quarterly reporting
- **Fund Administrators** — access filings, compliance reports, and company-level allocation data through conversational AI


## Available Tools
- **check_decilehub_status**: Verify connectivity
- **get_company**: Get company details
- **get_filing_report**: Get filing report
- **get_fund_performance**: Get fund performance
- **get_fund**: Get fund details
- **get_investor**: Get investor details
- **list_companies_by_fund**: List companies by fund
- **list_portfolio_companies**: List portfolio companies
- **list_filings**: List filings
- **list_funds**: List funds
- **list_investors**: List investors (LPs)
- **list_valuations**: List company valuations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DecileHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the performance metrics for our Fund III and compare against industry benchmarks."

**🤖 AI Agent:**
> Found Fund III (ID: fund_2019_a). Fetching performance data... Net IRR: 28.4% (top quartile benchmark: 22.1%). TVPI: 2.3x (median: 1.6x). DPI: 0.8x (distributions started Q3 2023). The fund is outperforming its 2019 vintage peers by 6.3 percentage points on IRR. 14 portfolio companies, $185M AUM. Would you like to see the company-by-company allocation?

---

**👤 You:**
> "List all portfolio companies in Fund II and show their current valuations."

**🤖 AI Agent:**
> Fund II (ID: fund_2017_b) has 11 portfolio companies. Top 5 by current valuation: 1) 'NeuralPath AI' — $142M (entry: $18M, 7.9x MOIC). 2) 'CloudForge' — $98M (entry: $12M, 8.2x). 3) 'DataVault' — $67M (entry: $15M, 4.5x). 4) 'GreenGrid Energy' — $54M (entry: $20M, 2.7x). 5) 'MedSync Health' — $41M (entry: $10M, 4.1x). Total portfolio unrealized value: $487M. Would you like the full valuation history for any company?

---

**👤 You:**
> "Show me all our LPs and their total commitments across all funds."

**🤖 AI Agent:**
> You have 23 LPs across all funds. Top 5 by total commitments: 1) 'Nordic Pension Fund' — $45M across Fund I, II, III. 2) 'Pacific Family Office' — $32M across Fund II, III. 3) 'Alpine Endowment' — $28M across Fund I, III. 4) 'Meridian Insurance Corp' — $25M in Fund III only. 5) 'Dr. Marcus Chen (Individual)' — $18M across Fund I, II. Total capital committed across all LPs: $312M. Would you like distribution histories for any specific LP?


## Installation & Usage

To install and use the **DecileHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decilehub](https://vinkius.com/mcp/decilehub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
