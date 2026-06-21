# PG&E Public Datasets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pge-public-datasets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access PG&E public energy data: monthly usage, billing, savings, and regional comparisons.

## Description
Access **PG&E Public Datasets** directly from any AI agent and explore energy consumption, billing trends, efficiency savings, and regional comparisons without any authentication.

### What you can do
- **Monthly Usage** — Get monthly electricity and gas consumption by ZIP code and customer segment
- **Customer Segments** — View energy usage breakdown across Residential, Commercial, Industrial, and Agricultural sectors
- **Yearly Trends** — Analyze year-over-year energy consumption trends
- **Electricity by ZIP** — Access ZIP code-level electricity consumption data
- **Gas by ZIP** — Access ZIP code-level natural gas consumption data
- **Billing Data** — Retrieve average bills and cost metrics by region
- **Savings Data** — Analyze energy efficiency program savings and cost-effectiveness
- **Regional Comparisons** — Compare energy usage across multiple ZIP codes side-by-side

### How it works
1. Subscribe to this server
2. No API key needed — completely free and public
3. Start exploring PG&E energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Energy Researchers** — analyze consumption trends and efficiency program effectiveness
- **Policy Makers** — understand energy affordability and regional consumption disparities
- **Clean Energy Companies** — identify high-consumption areas for solar/EV product targeting
- **Journalists** — access public energy data for reporting and analysis


## Available Tools (8)
- **get_billing_data**: Data is available by ZIP code and customer segment. Use this to analyze energy affordability, compare costs across regions, or identify rate impact on customers. Optional zipCode and year filters.

Get billing data and average costs from PG&E public datasets
- **get_usage_by_customer_type**: Shows total consumption for Residential, Commercial, Industrial, and Agricultural sectors. Use this to understand the energy consumption distribution across different customer categories. Optional dataType ("electric"/"gas") and year filters.

Get energy usage broken down by customer segment (residential, commercial, industrial, agricultural)
- **compare_regions**: Returns side-by-side usage figures (kWh and therms), customer counts, and average bills for each region. Use this to identify regional differences in energy consumption, support geographic targeting for efficiency programs, or compare urban vs. rural usage patterns. ZIP codes are comma-separated (e.g., "94102,94103,94104"). Optional dataType and year filters.

Compare energy usage data between multiple ZIP codes/regions
- **get_electricity_by_zip**: Returns monthly or annual usage figures broken down by geographic area. Use this to compare electricity usage across neighborhoods, identify high-consumption areas, or support energy efficiency targeting. Optional year filter.

Get electricity consumption data for specific ZIP codes in PG&E service area
- **get_gas_by_zip**: Returns monthly or annual gas usage figures by geographic area. Use this to analyze heating demand patterns, compare gas usage across regions, or identify electrification opportunities. Optional year filter.

Get natural gas consumption data for specific ZIP codes in PG&E service area
- **get_monthly_usage**: Data is organized by ZIP code, month, year, and customer segment (Residential, Commercial, Industrial, Agricultural). Returns kWh for electric and therms for gas. Use this to analyze consumption patterns over time. Optional filters: dataType ("electric" or "gas"), customerType, zipCode (5-digit), and year (YYYY).

Get monthly energy consumption data by ZIP code and customer segment from PG&E public datasets
- **get_savings_data**: Includes program participation counts, kWh/therms saved, program costs, and cost-effectiveness metrics by program type. Use this to evaluate program ROI, compare effectiveness across initiatives, or identify high-impact efficiency strategies. Optional programType and year filters.

Get energy efficiency program savings data from PG&E
- **get_yearly_trends**: Shows how electricity and gas usage has changed over multiple years. Use this to identify long-term patterns, growth/decline in energy demand, and seasonal variations. Optional dataType filter ("electric" or "gas").

Get yearly energy consumption trends from PG&E public data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PG&E Public Datasets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show monthly electricity usage by customer type."

**🤖 AI Agent:**
> Monthly electricity usage breakdown: Residential avg 650 kWh/month ($95), Commercial avg 4,200 kWh/month ($580), Industrial avg 45,000 kWh/month ($4,800), Agricultural avg 12,000 kWh/month ($1,100). Residential represents 35% of total consumption, Commercial 40%, Industrial 15%, Agricultural 10%.

---

**👤 You:**
> "Compare ZIP codes 94102, 94301, and 95054."

**🤖 AI Agent:**
> Regional comparison: 94102 (SF Mission): 5.2M kWh/month, 42K customers, avg $138 bill. 94301 (Palo Alto): 4.8M kWh/month, 28K customers, avg $165 bill. 95054 (Santa Clara): 6.1M kWh/month, 35K customers, avg $152 bill. Palo Alto has highest per-customer usage despite fewer customers, likely due to larger homes and higher income.

---

**👤 You:**
> "Show yearly energy consumption trends."

**🤖 AI Agent:**
> Yearly trends (2020-2024): 2020: 82,400 GWh (pandemic dip), 2021: 85,100 GWh (+3.3%), 2022: 87,800 GWh (+3.2%), 2023: 86,200 GWh (-1.8%, mild weather), 2024: 89,500 GWh (+3.8%, data center growth). Gas trends: declining 2% annually due to electrification and heat pump adoption.


## ❓ FAQ

**Q: Is any authentication required?**
No! All PG&E Public Datasets are completely free and accessible without any API key or authentication. Just subscribe and start querying energy data immediately.

**Q: What customer segments are available?**
PG&E provides data for four customer segments: Residential (homes), Commercial (businesses), Industrial (manufacturing), and Agricultural (farming). Each segment has different consumption patterns and billing structures.

**Q: Can I compare multiple ZIP codes?**
Yes! Use the compare_regions tool with comma-separated ZIP codes (e.g., "94102,94103,94104"). It returns side-by-side usage data, customer counts, and average bills for each region, making it easy to identify geographic differences in energy consumption.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pge-public-datasets](https://vinkius.com/mcp/pge-public-datasets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PG&E Public Datasets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pge-public-datasets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PG&E Public Datasets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pge-public-datasets": {
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
