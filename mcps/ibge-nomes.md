# IBGE Nomes MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-nomes)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-nomes-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-nomes-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian name frequency and ranking data from IBGE — explore popularity by decade, gender, and locality.

## Description
Connect to the **IBGE (Brazilian Institute of Geography and Statistics)** database through any AI agent to explore the rich demographic history of Brazilian names. This server provides direct access to the 'Nomes no Brasil' census data.

### What you can do

- **Name Frequency** — Query the number of births per decade for specific names (e.g., 'MARIA' or 'ENZO') to see how trends evolved over time.
- **Rankings & Popularity** — Generate rankings of the most frequent names in Brazil, with optional filters for gender and specific decades.
- **Geographic Insights** — Filter results by locality ID to understand regional naming preferences across different Brazilian states and municipalities.
- **Comparative Analysis** — Use the pipe separator to compare multiple names simultaneously and identify cultural shifts.

### How it works

1. Subscribe to this server
2. No API key is required as it uses the public IBGE Open Data API
3. Start querying Brazilian name statistics from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts & Sociologists** — study naming trends and demographic shifts in the Brazilian population.
- **Content Creators & Writers** — find historically accurate names for characters based on specific decades in Brazil.
- **Developers** — integrate official Brazilian demographic data into applications without complex setup.


## Available Tools
- **get_name_frequency**: Multiple names can be separated by a pipe (|).

Obtains the frequency of births per decade for a specific name
- **get_names_ranking**: Obtains a ranking of the most frequent names according to specified filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Nomes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the birth frequency of the name 'Neymar' in Brazil per decade?"

**🤖 AI Agent:**
> I've queried the IBGE database for 'NEYMAR'. The name saw a significant rise in the 2000s with 4,685 occurrences, compared to only 436 in the 1990s. Would you like to see the ranking for the 2010s as well?

---

**👤 You:**
> "Show me the top 10 most popular female names in Brazil during the 1980s."

**🤖 AI Agent:**
> Fetching the 1980s ranking... The top female names were Maria, Ana, and Aline. Maria remains the most frequent with over 1.6 million registrations in that decade alone. Do you want to filter this by a specific state?

---

**👤 You:**
> "Compare the popularity of 'Enzo' and 'Valentina' using IBGE data."

**🤖 AI Agent:**
> Comparing 'ENZO' and 'VALENTINA'... Both names exploded in popularity in the 2000s. Enzo reached 44,056 registrations while Valentina reached 10,033 in the same period. Would you like to see which states have the highest density for these names?


## Installation & Usage

To install and use the **IBGE Nomes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-nomes](https://vinkius.com/mcp/ibge-nomes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
