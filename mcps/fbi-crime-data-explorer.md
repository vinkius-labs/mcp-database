# FBI Crime Data Explorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fbi-crime-data-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fbi-crime-data-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fbi-crime-data-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access official FBI crime statistics, including national estimates, state-level summaries, and agency-specific data via AI.

## Description
Connect to the **FBI Crime Data Explorer (CDE)** to retrieve comprehensive law enforcement statistics directly through natural language. This server provides access to the Uniform Crime Reporting (UCR) program's extensive datasets.

### What you can do

- **National Estimates** — Retrieve estimated crime totals for the entire United States across specific year ranges.
- **State Summaries** — Fetch detailed offense data (violent crime, property crime, etc.) for any specific US state.
- **Agency-Level Data** — Query statistics reported by specific local, county, or state law enforcement agencies using their unique ORI identifier.
- **Victim Demographics** — Analyze NIBRS data to see breakdowns of victims by age, race, and sex for various offenses.

### How it works

1. Subscribe to this server
2. Enter your FBI CDE API Key
3. Start querying public safety data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts & Researchers** — quickly pull structured crime data for academic or professional reports.
- **Journalists** — verify crime statistics and trends for specific regions or agencies instantly.
- **Policy Makers** — evaluate the impact of safety initiatives using official historical data.


## Available Tools
- **get_agency_summarized**: Retrieve crime data for a specific law enforcement agency
- **get_national_estimates**: Retrieve national crime estimates
- **get_nibrs_victim_demographics**: Retrieve NIBRS victim demographic data
- **get_state_summarized**: Retrieve crime statistics for a specific state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FBI Crime Data Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me national crime estimates from 2015 to 2020."

**🤖 AI Agent:**
> I've retrieved the national estimates. From 2015 to 2020, violent crime saw a peak in 2016 with approximately 1.28 million incidents, followed by a gradual decline until 2019. Would you like a breakdown by specific offense type?

---

**👤 You:**
> "Get summarized burglary data for California (CA) between 2018 and 2022."

**🤖 AI Agent:**
> Accessing California state data... For the period 2018-2022, burglary rates showed a downward trend, starting at X incidents in 2018 and reaching Y in 2022. Do you want to see how this compares to the national average?

---

**👤 You:**
> "What is the age breakdown of robbery victims in New York?"

**🤖 AI Agent:**
> Querying NIBRS demographics for New York... The data shows that the largest group of robbery victims falls within the 25-34 age range, accounting for approximately 28% of reported incidents. Would you like to see the breakdown by race or sex instead?


## Installation & Usage

To install and use the **FBI Crime Data Explorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fbi-crime-data-explorer](https://vinkius.com/mcp/fbi-crime-data-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
