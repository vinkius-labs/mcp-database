# UK ONS Population — Deaths, Well-being & Demographics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uk-ons-population-deaths-well-being-demographics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uk-ons-population-deaths-well-being-demographics-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **UK ONS Population — Deaths, Well-being & Demographics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics](https://vinkius.com/mcp/uk-ons-population-deaths-well-being-demographics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
