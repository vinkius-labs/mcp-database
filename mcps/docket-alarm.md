# Docket Alarm MCP Server

Search over 732 million legal records, track court dockets, and extract AI-powered insights from PACER and state courts.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docket-alarm)

## Overview
**Category:** data-analytics
**Tools Count:** 13

## Description
Connect your **Docket Alarm** account to any AI agent to access one of the world's largest databases of legal records and court filings.

### What you can do

- **Comprehensive Search** — Query over 732 million records using boolean and fielded searches via the `search` tool.
- **Direct PACER Access** — Search federal courts directly using `search_pacer` to get the most up-to-date litigation data.
- **Docket Management** — Retrieve full docket information with `get_docket` and set up automated alerts for new activity using `track_case`.
- **AI Legal Analysis** — Automatically summarize complex legal documents with `get_complaint_summary` or extract specific results using `extract_judgment`.
- **State & Agency Courts** — Access specialized state and agency courts using `search_direct` after identifying required arguments with `get_search_direct_args`.

### How it works

1. Subscribe to this server
2. Enter your Docket Alarm Username and Password
3. Start researching litigation and tracking cases directly from Claude, Cursor, or any MCP-compatible client

Stop manually checking court websites for updates. Your AI agent now serves as a high-powered paralegal and legal researcher.

### Who is this for?

- **Litigators & Attorneys** — Instantly find relevant case law and track opposing counsel's filings across multiple jurisdictions.
- **Legal Researchers** — Perform deep-dive boolean searches across hundreds of millions of records without leaving your workflow.
- **Corporate Legal Teams** — Monitor litigation trends and receive real-time alerts on cases affecting your organization.


## Available Tools
- **ask_docket**: Ask natural language questions about a specific docket (VIDA AI)
- **match_case**: Find cases using partial information (VIDA AI)
- **get_cause_of_action**: Identify causes of action and relevant statutes (VIDA AI)
- **get_complaint_summary**: Extract long or short summaries of complaints (VIDA AI)
- **get_docket**: Set cached=False to fetch live from the court (PACER fees may apply).

Retrieve full docket information
- **get_search_direct_args**: Get required arguments for a direct court search
- **extract_judgment**: Extract judgments and outcomes from cases (VIDA AI)
- **list_search_direct_courts**: List supported courts for direct search
- **search_direct**: Search state and agency courts directly
- **search_pacer**: Note: Incurs a $0.10 fee per page of results unless test=true.

Search PACER/Federal courts directly
- **search**: Search Docket Alarm database
- **smart_search**: Generate complex search queries from natural language instructions (VIDA AI)
- **track_case**: Set up alerts for new activity on a docket


## Installation & Usage

To install and use the **Docket Alarm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docket-alarm](https://vinkius.com/mcp/docket-alarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
