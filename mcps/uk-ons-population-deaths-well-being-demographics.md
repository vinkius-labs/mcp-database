# UK ONS Population — Deaths, Well-being & Demographics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

UK population and health statistics: weekly death registrations by age, sex, and region, personal well-being estimates (life satisfaction, happiness, anxiety), suicide data by local authority, and population projections from the ONS.

## Description
UK population and health data.

### What you can do
- **Weekly Deaths** — By age, sex, and region
- **Well-being** — Life satisfaction, happiness, anxiety
- **Suicides** — By local authority
- **Projections** — Population forecasts to 2043


## Available Tools (5)
- **get_weekly_deaths**: Datasets: weekly-deaths-age-sex (by age and sex), weekly-deaths-region (by region). National statistics updated weekly.

Get weekly death registrations in England and Wales — by age, sex, and region
- **get_wellbeing**: Dataset: wellbeing-quarterly. Higher scores (0-10) indicate better well-being (except anxiety, where lower is better).

Get UK personal well-being estimates — life satisfaction, happiness, anxiety
- **get_wellbeing_local**: Dataset: wellbeing-local-authority. Covers life satisfaction, worthwhileness, happiness, and anxiety by region.

Get well-being estimates by UK local authority
- **get_suicides**: Dataset: suicides-in-the-uk. National statistics. If you are struggling, call Samaritans free: 116 123.

Get suicide registrations by local authority in England and Wales
- **get_population_projections**: Dataset: projections-older-people-sex-ratios.

Get UK population projections for older people, sex ratios by local authority


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK ONS Population — Deaths, Well-being & Demographics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest weekly death figures for England and Wales?"

**🤖 AI Agent:**
> 📊 **Weekly Deaths — England & Wales**

Week ending 28 March 2026: 11,247 deaths
Previous week: 10,893
5-year average: 10,450

+7.6% above 5-year average

Source: ONS, weekly-deaths-age-sex

---

**👤 You:**
> "What are the latest figures for life satisfaction in the UK?"

**🤖 AI Agent:**
> For the latest reporting period, the average rating of life satisfaction in the UK was 7.45 out of 10. The proportion of people reporting 'very high' life satisfaction was approximately 25%.

---

**👤 You:**
> "Show me population forecasts for the UK up to 2045."

**🤖 AI Agent:**
> Based on ONS national population projections (principal projection), the UK population is projected to increase from 67.0 million to 71.0 million by mid-2045, reflecting an aging population with a lower birth rate.


## ❓ FAQ

**Q: How often is death data updated?**
Weekly. The ONS publishes provisional death registrations every Tuesday for the previous week, with a 11-day reporting lag.

**Q: Does it track personal well-being metrics?**
Yes, the ONS measures personal well-being across four indicators (O4): life satisfaction, feeling that the things done in life are worthwhile, happiness, and anxiety.

**Q: Are population figures based on the Census?**
The datasets include both decennial census data and mid-year population estimates, which are updated annually to account for births, deaths, and migration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics](https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK ONS Population — Deaths, Well-being & Demographics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-ons-population-deaths-well-being-demographics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK ONS Population — Deaths, Well-being & Demographics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-ons-population-deaths-well-being-demographics": {
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
