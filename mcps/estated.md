# Estated MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/estated)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/estated-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/estated-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access comprehensive US property data including ownership, assessment, and structural details directly from any AI agent.

## Description
Connect to **Estated** to retrieve deep property insights across the United States. This server allows your AI agent to query a massive database of real estate records using various address formats or parcel identifiers.

### What you can do

- **Flexible Address Search** — Look up properties using combined strings, split components, or highly structured parsed data.
- **Parcel Identification** — Query specific properties using County FIPS codes and Assessor's Parcel Numbers (APN).
- **Comprehensive Data** — Retrieve detailed information on ownership, property characteristics, tax assessments, and market values.
- **Data-Driven Decisions** — Empower your agent to analyze real estate trends or verify property details without leaving the chat.

### How it works

1. Subscribe to this server
2. Enter your Estated API Token
3. Start querying US property data from Claude, Cursor, or any MCP-compatible client.

### Who is this for?

- **Real Estate Professionals** — Quickly verify property ownership and assessment data.
- **Data Analysts** — Automate the retrieval of property characteristics for market research.
- **Developers** — Integrate reliable property data into workflows without complex API implementations.


## Available Tools
- **get_property_combined_address**: Get property data using a single combined address string
- **get_property_fips_apn**: Get property data using FIPS code and APN
- **get_property_parsed_address**: Get property data using detailed parsed address components
- **get_property_split_address**: Get property data using split address components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Estated** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get property details for 151 Battle Green Dr, Rochester, NY 14624."

**🤖 AI Agent:**
> I've retrieved the data for 151 Battle Green Dr. It's a single-family residence with 3 bedrooms and 2 bathrooms, built in 1972. The current owner is listed as [Name] and the last assessed value was $185,000.

---

**👤 You:**
> "Find property info using FIPS 36055 and APN 123-45-678."

**🤖 AI Agent:**
> Using the FIPS and APN provided, I found a commercial property in Monroe County. It has a total building area of 5,200 sq ft and is currently zoned for general business use.

---

**👤 You:**
> "Look up the property at 742 Evergreen Terrace in Springfield, IL."

**🤖 AI Agent:**
> I've located 742 Evergreen Terrace. This property features a lot size of 0.25 acres and includes structural details such as a finished basement and an attached garage.


## Installation & Usage

To install and use the **Estated** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/estated](https://vinkius.com/mcp/estated)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
