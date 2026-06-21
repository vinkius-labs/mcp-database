# GSA Per Diem Rates MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gsa-per-diem-rates)
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


## ❓ FAQ

**Q: How can I find the per diem rates for a specific city like Los Angeles?**
You can use the `get_rates_by_city` tool. Just provide the city name (Los Angeles), the state abbreviation (CA), and the fiscal year you are interested in.

**Q: Is it possible to get a breakdown of meal costs for the day?**
Yes! Use the `get_mie_breakdown` tool for a specific fiscal year. It returns the breakdown for Meals and Incidental Expenses (M&IE), showing allocations for breakfast, lunch, dinner, and incidentals.

**Q: Can I look up rates using just a ZIP code?**
Absolutely. The `get_rates_by_zip` tool allows you to input a 5-digit ZIP code and a fiscal year to retrieve the applicable per diem rates for that specific location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gsa-per-diem-rates](https://vinkius.com/mcp/gsa-per-diem-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GSA Per Diem Rates** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gsa-per-diem-rates` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GSA Per Diem Rates** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gsa-per-diem-rates": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
