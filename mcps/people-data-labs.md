# People Data Labs MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/people-data-labs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/people-data-labs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/people-data-labs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Enrich person and company profiles with B2B data — access millions of records for lead generation, identity resolution, and market intelligence.

## Description
Connect **People Data Labs** to your AI agent to access one of the most comprehensive B2B datasets available. Enrich profiles, identify prospects, and search through millions of person and company records using natural language.

### What you can do

- **Person Enrichment** — Retrieve full professional profiles using just an email, phone number, or social media URL (LinkedIn, Twitter, etc.).
- **Company Intelligence** — Get detailed company metadata, including industry, size, location, and stock tickers.
- **Advanced Search** — Query the entire Person or Company dataset using SQL or Elasticsearch DSL directly from your conversation.
- **Identity Resolution** — Identify multiple potential profiles associated with a set of attributes to find the best match.
- **Bulk Operations** — Enrich up to 100 person or company records in a single request for high-scale workflows.

### How it works

1. Subscribe to this server
2. Enter your People Data Labs API Key
3. Start enriching your CRM data or building lead lists from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & Marketing Teams** — Instantly enrich inbound leads or build targeted outbound lists without manual research.
- **Recruiters** — Find detailed candidate histories and contact information directly from your workflow.
- **Data Engineers** — Perform complex dataset queries and cleaning operations using SQL through an AI interface.


## Available Tools
- **pdl_autocomplete**: Get autocomplete suggestions for Search API query values
- **pdl_bulk_enrich_company**: Bulk enrich up to 100 companies
- **pdl_bulk_enrich_person**: Bulk enrich up to 100 persons
- **pdl_clean_company**: Clean and standardize raw company data
- **pdl_clean_location**: Clean and standardize raw location data
- **pdl_clean_school**: Clean and standardize raw school data
- **pdl_enrich_company**: Enrich a company profile
- **pdl_enrich_ip**: Enrich an IP address
- **pdl_enrich_job_title**: Enrich a job title to find similar titles and relevant skills
- **pdl_enrich_person**: Enrich a person profile using attributes
- **pdl_identify_person**: Returns match_score.

Identify multiple possible person profiles
- **pdl_search_company**: Provide either an Elasticsearch DSL query or a SQL query.

Search the Company Dataset using Elasticsearch DSL or SQL
- **pdl_search_job_posting**: Search active and historical job postings
- **pdl_search_person**: Provide either an Elasticsearch DSL query or a SQL query.

Search the Person Dataset using Elasticsearch DSL or SQL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **People Data Labs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the person profile for the email 'sean@peopledatalabs.com'."

**🤖 AI Agent:**
> I've found the profile for Sean Thorne. He is the Co-Founder and CEO at People Data Labs, based in San Francisco. Would you like to see his full work history or education details?

---

**👤 You:**
> "Search for companies in the 'Financial Services' industry with more than 1000 employees using SQL."

**🤖 AI Agent:**
> I've executed the SQL search. I found several companies matching your criteria, including 'Stripe', 'Plaid', and 'Brex'. Which one would you like to explore in detail?

---

**👤 You:**
> "Identify potential profiles for 'John Doe' who works at 'Google'."

**🤖 AI Agent:**
> I've identified 3 possible profiles for 'John Doe' at Google. One is a Software Engineer in Mountain View, another is a Product Manager in New York. Should I enrich the Software Engineer profile for you?


## Installation & Usage

To install and use the **People Data Labs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/people-data-labs](https://vinkius.com/mcp/people-data-labs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
