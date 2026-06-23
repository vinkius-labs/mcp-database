# WHO GHO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/who-gho)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access 2,200+ health indicators from 194 countries — life expectancy, disease prevalence, mortality rates, immunization coverage, and environmental health data from the World Health Organization.

## Description
Connect your AI agent to the **WHO Global Health Observatory** — the authoritative source for health statistics from all 194 member states of the World Health Organization.

### What you can do

- **Indicator Search** — Find among 2,200+ health indicators across topics: life expectancy, child mortality, HIV/AIDS, malaria, tuberculosis, obesity, mental health, immunization, water quality, air pollution, and more
- **Country-Level Data** — Retrieve time-series data for any indicator filtered by country (ISO-3 codes), with sex disaggregation where available
- **Country Health Profiles** — Get instant health snapshots for any country with key metrics: life expectancy, healthy life expectancy, child mortality, obesity prevalence, and alcohol consumption

### How it works

1. Subscribe to this server
2. Start querying global health data immediately — no API key required

### Who is this for?

- **Public Health Professionals** — monitor epidemiological trends and compare health outcomes across countries to inform policy decisions
- **Global Health Researchers** — retrieve standardized health statistics for academic studies and meta-analyses
- **International Development Agencies** — track progress toward Sustainable Development Goals (SDGs) with official WHO indicators


## Available Tools (3)
- **get_who_country_profile**: Use ISO-3 country codes (BRA, USA, JPN, DEU, IND).

Get a health snapshot for any country from WHO data
- **get_who_indicator_data**: Returns values by year with sex disaggregation where available. Use search_who_indicators first to find codes.

Get country-level data for a WHO health indicator
- **search_who_indicators**: Returns indicator codes for further data retrieval.

Search 2200+ global health indicators from the World Health Organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHO GHO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the life expectancy in Japan and how does it compare globally?"

**🤖 AI Agent:**
> Japan (JPN) health profile — Life expectancy at birth: 84.3 years (2021), consistently among the world's highest. Healthy life expectancy: 73.3 years. Women: 87.1 years, Men: 81.5 years. Additional indicators: Under-5 mortality rate: 2.5 per 1,000 live births (one of the lowest globally). Obesity prevalence: 4.3% (far below global average of 13.1%).

---

**👤 You:**
> "Search for WHO indicators related to tuberculosis worldwide."

**🤖 AI Agent:**
> Found 15+ TB-related indicators. Key ones include: MDG_0000000020 (TB incidence per 100K), MDG_0000000021 (TB prevalence per 100K), MDG_0000000022 (TB mortality per 100K), TB_c_newinc (new TB cases notified), TB_1 (TB treatment success rate). Use any indicator code with a country filter to get country-specific time-series data.

---

**👤 You:**
> "Give me a complete health snapshot for Brazil."

**🤖 AI Agent:**
> Brazil (BRA) health profile: Life expectancy: 75.9 years | Healthy life expectancy: 65.4 years | Under-5 mortality: 14.3 per 1,000 | Obesity prevalence (adults): 22.3% | Current health expenditure: 9.6% of GDP. Data sourced from WHO member state reports with the most recent available year for each indicator.


## ❓ FAQ

**Q: What health topics and indicators does the WHO GHO cover?**
The GHO covers 2,200+ indicators across 40+ themes: life expectancy, child and maternal mortality, infectious diseases (HIV, TB, Malaria, COVID-19), non-communicable diseases (cancer, diabetes, cardiovascular), mental health, immunization coverage, nutrition, water/sanitation, air quality, road safety, tobacco use, and the full Sustainable Development Goals (SDG) monitoring framework.

**Q: Is the WHO GHO API free and does it require authentication?**
Yes, the GHO OData API is completely free and open without any authentication. The data is published by the World Health Organization as a public good. There are no API keys, no registration, and no rate limits for reasonable usage. The data is updated regularly with the latest country reports.

**Q: Which countries are covered and what country codes should I use?**
All 194 WHO member states plus territories are covered. Use ISO-3 country codes: BRA (Brazil), USA (United States), GBR (United Kingdom), JPN (Japan), DEU (Germany), IND (India), CHN (China), FRA (France), AUS (Australia), ZAF (South Africa), etc. Data availability varies by indicator and country reporting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/who-gho](https://vinkius.com/mcp/who-gho)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WHO GHO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `who-gho` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WHO GHO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "who-gho": {
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
