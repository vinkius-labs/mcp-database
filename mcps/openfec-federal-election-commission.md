# OpenFEC (Federal Election Commission) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openfec-federal-election-commission)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openfec-federal-election-commission-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openfec-federal-election-commission-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time federal campaign finance data — search candidates, track committee filings, and analyze election financial totals directly.

## Description
Connect to the official **OpenFEC** API and bring transparency to federal election data through your AI agent. This server provides direct access to the Federal Election Commission's comprehensive database of campaign finance information.

### What you can do

- **Candidate Research** — List and search for individuals running for President, Senate, or House with filters for state, party, and cycle.
- **Financial Analytics** — Retrieve aggregated financial totals and summaries for specific candidates to understand fundraising and spending.
- **Committee Tracking** — Explore political committees (PACs, party committees) and their detailed metadata and filings.
- **Historical Context** — Access the history of candidate filings and designations over multiple election cycles.
- **Deep Metadata** — Fetch detailed profiles for any candidate or committee using their unique FEC identifiers.

### How it works

1. Subscribe to this server
2. Enter your OpenFEC API Key
3. Start querying election data from Claude, Cursor, or any MCP client

### Who is this for?

- **Journalists & Researchers** — quickly verify campaign finance figures and candidate statuses without manual database exports.
- **Data Analysts** — pull structured election data directly into your workflow for political trend analysis.
- **Civic Tech Developers** — integrate official government data into applications with ease.


## Available Tools
- **get_candidate_history**: Get the history of a candidate filings and designations
- **get_candidate**: Get detailed information for a specific candidate by ID
- **get_candidate_totals**: Get aggregated financial totals for a specific candidate
- **get_committee_history**: Get the history of a committee characteristics over time
- **get_committee**: Get detailed information for a specific committee by ID
- **get_totals_by_committee_type**: Get financial totals for a specific committee type
- **get_totals_by_entity**: Get financial totals aggregated by candidate or committee entity
- **get_totals_officer_summary**: Summarize financial data by committee officer
- **list_candidates**: Fetch a list of candidates with various filters
- **list_committees**: Fetch a list of committees with filters
- **list_filings**: List all filings (electronic and paper) with filters
- **list_reports**: Fetch financial reports filed by specific types of committees
- **list_schedule_a**: Itemized Receipts: Contributions from individuals and committees
- **list_schedule_b**: Itemized Disbursements: Operating expenditures, transfers, refunds
- **list_schedule_c**: Loans: Information on loans received or made by committees
- **list_schedule_d**: Debts: Debts and obligations owed by or to committees
- **list_schedule_e**: Independent Expenditures: Spending to support/oppose candidates
- **list_schedule_f**: Coordinated Party Expenditures: Spending in coordination with candidates
- **list_state_election_offices**: Get contact information for state election offices
- **search_candidates**: Search for candidates by name or other attributes
- **search_committees**: Search for committees by name or ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenFEC (Federal Election Commission)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all presidential candidates for the 2024 election cycle."

**🤖 AI Agent:**
> I've retrieved the list of presidential candidates for 2024. There are currently several registered candidates, including [Candidate Name] (ID: P...) and [Candidate Name] (ID: P...). Would you like to see the financial totals for any of them?

---

**👤 You:**
> "Show me the financial totals for candidate ID P00000001 in the 2024 cycle."

**🤖 AI Agent:**
> For the 2024 cycle, candidate P00000001 has reported total receipts of $X,XXX,XXX and total disbursements of $Y,XXX,XXX. They currently have $Z,XXX,XXX cash on hand. Do you need a breakdown of individual committee contributions?

---

**👤 You:**
> "Search for political committees with 'Action' in their name."

**🤖 AI Agent:**
> I found several committees matching 'Action'. Notable ones include 'Climate Action PAC' (ID: C...) and 'Justice Action Fund' (ID: C...). Which one would you like to inspect for detailed filings?


## Installation & Usage

To install and use the **OpenFEC (Federal Election Commission)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfec-federal-election-commission](https://vinkius.com/mcp/openfec-federal-election-commission)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
