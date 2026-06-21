# GSA Per Diem Rates MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gsa-per-diem-rates)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gsa-per-diem-rates-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gsa-per-diem-rates-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access official U.S. government per diem rates for lodging and meals by city, state, or ZIP code directly from your AI agent.

## Description
Connect to the **GSA Per Diem Rates** server to instantly retrieve federal travel reimbursement data. This tool allows AI agents to query the official U.S. General Services Administration database for accurate lodging and meal rates.

### What you can do

- **City & State Lookups** — Get precise rates for specific destinations like 'Fairfax, VA' for any fiscal year.
- **ZIP Code Queries** — Quickly find rates using a 5-digit ZIP code to ensure location accuracy.
- **M&IE Breakdowns** — Access detailed Meals and Incidental Expenses (M&IE) data, including breakfast, lunch, and dinner allocations.
- **Statewide Data** — Retrieve all county and city rates within a specific state for broader travel planning.
- **CONUS Lodging** — Fetch standard continental United States lodging rates for general budgeting.

### How it works

1. Subscribe to this server
2. Enter your GSA API Key
3. Ask about travel rates for any US location

### Who is this for?

- **Finance & Accounting Teams** — Automate the verification of travel expense reports against federal standards.
- **Government Contractors** — Ensure compliance with federal travel regulations during project bidding and billing.
- **Travel Coordinators** — Quickly calculate travel budgets for employees across different US regions.


## Available Tools
- **get_conus_lodging**: Get CONUS lodging rates for a specific year
- **get_mie_breakdown**: Get M&IE breakdown rates for a specific year
- **get_rates_by_city**: Get per diem rates for a specific city and state
- **get_rates_by_state**: Get per diem rates for all counties and cities in a state
- **get_rates_by_zip**: Get per diem rates for a specific ZIP code
- **get_zip_mapping**: Useful for high volume requests.

Get ZIP code to DID mapping for a specific year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GSA Per Diem Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the per diem rates for Fairfax, VA in 2025?"

**🤖 AI Agent:**
> For Fairfax, Virginia in fiscal year 2025, the lodging rate is $193/night (Oct-Sep). The M&IE rate is $76 per day. Would you like the breakdown for the first and last day of travel?

---

**👤 You:**
> "Show me the meal and incidental expense breakdown for fiscal year 2025."

**🤖 AI Agent:**
> I've retrieved the M&IE breakdown for 2025. For a $76 total: Breakfast is $18, Lunch is $19, Dinner is $34, and Incidentals are $5. The first/last day of travel rate is $57.00.

---

**👤 You:**
> "Get the lodging rates for ZIP code 90210 for 2025."

**🤖 AI Agent:**
> Searching for ZIP 90210 (Beverly Hills, CA)... For fiscal year 2025, the lodging rates range from $200 to $280 depending on the month. The M&IE rate is $76. Would you like the monthly lodging schedule?


## Installation & Usage

To install and use the **GSA Per Diem Rates** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gsa-per-diem-rates](https://vinkius.com/mcp/gsa-per-diem-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
