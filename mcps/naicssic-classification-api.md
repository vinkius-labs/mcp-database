# NAICS/SIC Classification API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/naicssic-classification-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/naicssic-classification-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/naicssic-classification-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Search industry codes — audit NAICS and SIC via AI.

## Description
Empower your AI agent to orchestrate your entire market research and industry auditing workflow with the **NAICS/SIC Classification API**, the authoritative source for standardized business classification data. By connecting the Brand.dev classification service to your agent, you transform complex industry searches into a natural conversation. Your agent can instantly retrieve NAICS and SIC codes, audit industry titles, and query specific classification metadata without you ever touching a technical portal. Whether you are conducting competitive analysis or managing regional data constraints, your agent acts as a real-time market consultant, ensuring your data is always verified and precise.

### What you can do

- **Code Auditing** — Search for thousands of NAICS and SIC codes by keyword and retrieve high-resolution metadata, including titles and descriptions.
- **Industry Oversight** — Audit the hierarchical distribution of classification codes to understand the current industry lead in market segmentation instantly.
- **Metadata Intelligence** — Retrieve unique identifiers and category markers for any record to assist in deep-dive archival classification.
- **Classification Discovery** — Identify relevant industry markers for your business development or research projects through natural language interaction.
- **Operational Monitoring** — Check API status to ensure your market research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Brand.dev API Key
3. Start managing your industry intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers & Analysts** — monitor industry trends and retrieve official metadata straight from your workflow.
- **Business Development Leads** — verify classification codes and audit segmentation patterns without manual searching.
- **Data Architects** — perform rapid audits of industry markers and identify relevant data patterns through natural language.
- **Operations Leads** — automate technical data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_api_status**: dev Classification API.

Check if the NAICS/SIC service is operational
- **get_classification_details**: Get full metadata and description for a specific NAICS or SIC code
- **search_naics_codes**: Search for NAICS (North American Industry Classification System) codes
- **search_sic_codes**: Search for SIC (Standard Industrial Classification) codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NAICS/SIC Classification API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for NAICS codes related to 'software' using Brand.dev."

**🤖 AI Agent:**
> I've retrieved several NAICS codes related to software! Notable entries include 511210 (Software Publishers) and 541511 (Custom Computer Programming Services). Would you like the full descriptions for any of these codes?

---

**👤 You:**
> "What is the industry for SIC code '7371'?"

**🤖 AI Agent:**
> I've identified the industry for SIC 7371! It is categorized as 'Computer Programming Services'. I can provide the full description and related NAICS markers to help you in your classification audit.

---

**👤 You:**
> "Search for SIC codes matching 'manufacturing'."

**🤖 AI Agent:**
> I've scanned the SIC catalog for manufacturing! I've identified several matching codes, including those for electronics and machinery production. I can provide the full metadata for any of these identifiers to help you in your research.


## Installation & Usage

To install and use the **NAICS/SIC Classification API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/naicssic-classification-api](https://vinkius.com/mcp/naicssic-classification-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
