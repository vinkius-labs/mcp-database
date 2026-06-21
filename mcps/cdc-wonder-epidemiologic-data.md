# CDC WONDER (Epidemiologic Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cdc-wonder-epidemiologic-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cdc-wonder-epidemiologic-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cdc-wonder-epidemiologic-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access public health data from the CDC WONDER system, including mortality, births, and vaccine adverse events directly through your AI agent.

## Description
Connect to the **CDC WONDER** (Wide-ranging Online Data for Epidemiologic Research) system to query massive public health databases through natural language.

### What you can do

- **Mortality Data** — Query the D76 (Detailed Mortality) and D77 (Underlying Cause of Death) databases for specific timeframes and regions.
- **Birth Statistics** — Access the D10 (Natality) database to analyze birth rates and maternal health metrics.
- **Vaccine Safety** — Query the VAERS (Vaccine Adverse Event Reporting System) database for safety monitoring data.
- **Structured Queries** — Execute complex ad-hoc queries using standard CDC parameters (B_, M_, V_, F_, O_ prefixes) for precise data extraction.
- **Epidemiologic Research** — Retrieve raw data for analysis in scientific research, public health policy, or educational projects.

### How it works

1. Subscribe to this server
2. Enter your CDC WONDER API Access Token (if required by your proxy) or accept the Data Use Agreement
3. Start querying epidemiologic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Epidemiologists & Researchers** — quickly pull mortality and birth statistics without navigating the complex WONDER web interface
- **Public Health Officials** — monitor health trends and vaccine safety reports directly from an AI assistant
- **Data Scientists** — fetch structured JSON epidemiologic data for integration into larger analytical workflows


## Available Tools
- **query_wonder_database**: g., D76 for Mortality). Provide the database ID and a JSON object of parameters (B_, M_, V_, F_, O_ prefixes).

Query CDC WONDER epidemiologic databases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CDC WONDER (Epidemiologic Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Query the CDC WONDER D76 database for mortality rates in 2021 with parameters for age groups."

**🤖 AI Agent:**
> I've initiated a request to the D76 Detailed Mortality database. The query is processing with your specified age group filters and 2021 timeframe. I will present the resulting epidemiologic table once the CDC system responds.

---

**👤 You:**
> "Fetch VAERS reports related to vaccine code 'COVID19' from the CDC WONDER database."

**🤖 AI Agent:**
> Accessing the VAERS database... I am executing `query_wonder_database` with the 'VAERS' ID and filtering for the 'COVID19' vaccine code. I'll summarize the reported adverse events and counts for you.

---

**👤 You:**
> "Analyze birth statistics for the state of California using database D10."

**🤖 AI Agent:**
> Querying the D10 Natality database for California. I'm applying the necessary location filters (F_ prefixes) to extract birth rates and maternal demographics. One moment while I retrieve the data.


## Installation & Usage

To install and use the **CDC WONDER (Epidemiologic Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cdc-wonder-epidemiologic-data](https://vinkius.com/mcp/cdc-wonder-epidemiologic-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
