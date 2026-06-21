# KnowFirst MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knowfirst)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/knowfirst-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/knowfirst-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query data intelligence — search entities, audit signals, and track market trends.

## Description
Connect your AI agent to **KnowFirst**, the leading provider of real-time data intelligence and entity profiling.

### Key Capabilities

- **Entity Profiling** — Deep search for companies and individuals to get comprehensive intelligence data
- **Signal Auditing** — Track changes and signals for specific entities over time to detect shifts in behavior
- **Market Analysis** — Access trending signals by category to understand sector-wide movements
- **Relationship Mapping** — Graph connections between entities to discover hidden networks and dependencies
- **Source Transparency** — Audit the data sources providing information for your research

### Simple Integration

1. Get your KnowFirst API Key from your dashboard
2. Configure the key in this MCP server
3. Start extracting data intelligence using natural language commands


## Available Tools
- **search_intelligence_entities**: Returns unique entity IDs.

Search for specific entities in the intelligence database
- **get_entity_profile**: Get complete intelligence profile for an entity
- **list_intelligence_sources**: g., Public Records, Social Signals, News).

List all data sources used by KnowFirst
- **query_custom_intelligence**: Provide the query parameters as a JSON string.

Execute a custom intelligence query
- **audit_entity_changes**: Audit historical changes for an entity
- **list_entity_data_points**: List raw data points for an entity
- **get_market_intelligence_trends**: g., Tech, Finance).

Get current market trends by category
- **search_data_sources**: Search for specific data sources
- **get_entity_connections**: Graph the connections of an entity
- **check_knowfirst_api_status**: Check the status of the KnowFirst API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KnowFirst** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Research Acme Corp in KnowFirst"

**🤖 AI Agent:**
> I've found Acme Corp (ID: ent_123). It has a very high confidence score. Intelligence shows a recent expansion in Europe and a positive news sentiment trend. Would you like to audit their connections?

---

**👤 You:**
> "Show me the connections for entity 'ent_123'"

**🤖 AI Agent:**
> Mapping relationships for 'ent_123'… I found 8 strong connections, including 3 parent companies and 5 strategic partners. I've highlighted the most critical nodes for your review.

---

**👤 You:**
> "What are the trending signals in the 'Fintech' category?"

**🤖 AI Agent:**
> The Fintech sector is currently showing a surge in 'Regulatory Change' signals and a decline in 'Early-stage Funding' reports. Most activity is concentrated in the US and Brazil.


## Installation & Usage

To install and use the **KnowFirst** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knowfirst](https://vinkius.com/mcp/knowfirst)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
