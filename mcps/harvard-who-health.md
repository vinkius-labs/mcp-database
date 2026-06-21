# Harvard WHO Health MCP Server

Access WHO global health indicators, disease statistics, and population health data for evidence-based research and policy analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/harvard-who-health)

## Overview
**Category:** data-analytics
**Tools Count:** 16

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


## Installation & Usage

To install and use the **Harvard WHO Health** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvard-who-health](https://vinkius.com/mcp/harvard-who-health)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
