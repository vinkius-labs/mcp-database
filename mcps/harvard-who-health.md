# Harvard WHO Health MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvard-who-health)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access WHO global health indicators, disease statistics, and population health data for evidence-based research and policy analysis.

## Description
Connect to the **WHO Global Health Observatory (GHO) API** — the world's most comprehensive source of global health statistics.

### What you can do

- **Health Indicators** — Search 1000+ indicators across all health domains
- **Life Expectancy** — Track life expectancy at birth by country
- **Immunization** — DTP3, measles, polio, BCG, and hepatitis B coverage
- **Infectious Diseases** — HIV/AIDS prevalence, TB incidence, malaria estimates
- **NCDs** — Diabetes, obesity, hypertension, tobacco, and alcohol data
- **Maternal Health** — Maternal mortality ratios and reproductive health
- **Health Workforce** — Physicians, nurses, dentists, pharmacists per 10,000 pop.
- **Health Expenditure** — Per capita spending in PPP dollars
- **Water & Sanitation** — WASH indicators for safe water and sanitation
- **Country Comparison** — Compare any indicator across multiple countries

### Who is this for?

- **Public Health Researchers** — global health trends and burden of disease
- **Epidemiologists** — disease surveillance and outbreak analysis
- **Policy Makers** — evidence-based health policy decisions
- **Global Health Students** — coursework and thesis research


## Available Tools
- **compare_countries**: Provide a comma-separated list of ISO 3-letter country codes. Returns the most recent 10 years of data for each country.

Compare a health indicator across countries
- **get_countries**: Returns ISO codes and country names for use with other indicator queries.

Get list of WHO member countries
- **get_dimensions**: Useful for understanding how to filter and disaggregate health data.

Get WHO data dimensions metadata
- **get_health_expenditure**: This indicator measures how much each country spends on healthcare, adjusted for purchasing power.

Get health expenditure data
- **get_health_workforce**: Supported types: "physicians", "nurses", "dentists", "pharmacists".

Get health workforce density data
- **get_hiv_aids**: Tracks the percentage of the population living with HIV, a critical indicator for public health programs and resource allocation.

Get HIV/AIDS prevalence data
- **get_immunization**: Supported shortcuts: "dtp3" (diphtheria-tetanus-pertussis), "measles", "polio", "bcg", "hepb3". Or use a WHO indicator code directly.

Get immunization coverage data
- **get_indicator_data**: g. "USA", "BRA", "GBR", "CHN", "IND"). Returns country, year, value, confidence intervals, and sex disaggregation.

Get time-series data for a WHO indicator
- **get_life_expectancy**: This is one of the most fundamental indicators of population health.

Get life expectancy data
- **get_malaria**: Essential for tracking the global burden of malaria, particularly in sub-Saharan Africa and Southeast Asia.

Get malaria case estimates
- **get_maternal_health**: This measures the number of maternal deaths per 100,000 live births, a critical indicator of reproductive health and healthcare quality.

Get maternal mortality data
- **get_mortality**: Common indicator codes: "NCDMORT3070" (NCD mortality), "CHILDMORTALITY" (under-5), "MATERNALMORTALITY". Use search_indicators to find specific codes.

Get mortality data by cause
- **get_ncd**: Supported shortcuts: "diabetes" (prevalence), "obesity" (BMI ≥30), "blood_pressure" (hypertension), "tobacco" (smoking), "alcohol" (consumption). Or use a WHO code.

Get non-communicable disease data
- **get_tuberculosis**: TB remains one of the top infectious disease killers worldwide, and this data tracks progress toward elimination.

Get tuberculosis incidence data
- **get_water_sanitation**: Supported types: "water" (safely managed drinking water), "sanitation" (safely managed sanitation), "hygiene" (basic hygiene facilities).

Get water and sanitation data
- **search_indicators**: Returns indicator codes and names. Use the indicator code with get_indicator_data to retrieve time-series data.

Search 1000+ WHO health indicators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvard WHO Health** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare life expectancy between USA, Brazil, Japan, and Nigeria"

**🤖 AI Agent:**
> I've compared life expectancy at birth across these four countries using WHO data, showing trends over the past decade.

---

**👤 You:**
> "Show diabetes prevalence data for India"

**🤖 AI Agent:**
> I've retrieved WHO diabetes prevalence data for India, showing time-series trends in blood glucose levels and diabetes rates among adults.

---

**👤 You:**
> "Get measles immunization coverage for sub-Saharan African countries"

**🤖 AI Agent:**
> I've retrieved measles immunization coverage from WHO for sub-Saharan African countries, showing DTP3 and MCV1 coverage percentages and year-over-year progress.


## ❓ FAQ

**Q: Do I need an API key?**
No. The WHO GHO API is completely free and public. No authentication required.

**Q: How many countries does WHO track?**
The WHO Global Health Observatory tracks health data for all 194 Member States, plus territories and regions. Data spans from the 1990s to the present with annual updates.

**Q: What types of health data are available?**
Over 1,000 indicators across mortality, morbidity, immunization, NCDs (diabetes, obesity), infectious diseases (HIV, TB, malaria), maternal health, health workforce, expenditure, water and sanitation, and more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvard-who-health](https://vinkius.com/mcp/harvard-who-health)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvard WHO Health** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `harvard-who-health` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvard WHO Health** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvard-who-health": {
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
