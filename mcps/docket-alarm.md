# Docket Alarm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docket-alarm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docket-alarm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docket-alarm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search over 732 million legal records, track court dockets, and extract AI-powered insights from PACER and state courts.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docket Alarm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Docket Alarm for cases involving '3M' with 'docket' in the query."

**🤖 AI Agent:**
> I've found several records for '3M'. The most recent is '3M Company v. New England Teamsters' (Docket: 1:23-cv-12345) filed in the District of Delaware. Would you like to see the full docket?

---

**👤 You:**
> "Get the full docket for case 1:23-cv-10001 in the 'cand' court."

**🤖 AI Agent:**
> Retrieving docket 1:23-cv-10001 from Northern District of California (cand)... I have the full list of 45 filings, including the initial complaint and the latest scheduling order. Which filing should I inspect?

---

**👤 You:**
> "Summarize the complaint for docket 1:22-cv-00500 in 'nysd'."

**🤖 AI Agent:**
> Analyzing the complaint... This is a copyright infringement suit where the plaintiff alleges unauthorized use of photographic works. The primary cause of action is under 17 U.S.C. § 501. Would you like the list of specific exhibits mentioned?


## Installation & Usage

To install and use the **Docket Alarm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docket-alarm](https://vinkius.com/mcp/docket-alarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
