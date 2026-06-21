# Proxycurl (LinkedIn Data) MCP Server

Enrich company and professional data via Proxycurl — lookup websites, funding history, employee profiles, and competitive intelligence directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/proxycurl-linkedin-data)

## Overview
**Category:** sales-automation
**Tools Count:** 18

## Description
Connect **Proxycurl** to your AI agent to access real-time B2B intelligence and LinkedIn-derived data. This server provides a powerful suite of tools for sales, recruitment, and market research.

### What you can do

- **Company Intelligence** — Resolve company names to websites, fetch logos, and retrieve deep metadata including industry and leadership using `company_website_lookup` and `get_company_details`.
- **Financial Insights** — Access complete funding histories, investment rounds, and participating investors for private and public companies via `get_company_funding`.
- **People Data** — Enrich professional profiles from work emails or names with `get_employee_profile`, and search for employees within specific organizations using `search_employees`.
- **Market Analysis** — Identify competitors based on product similarity with `get_competitor_listing` and list probable customers or partners.
- **Monitoring** — Create and manage monitor feeds to track organizational changes over time using `create_monitor_feed`.

### How it works

1. Subscribe to this server
2. Enter your Proxycurl API Key
3. Start querying B2B data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & RevOps** — Automate lead enrichment and find decision-makers without manual searching.
- **Recruiters** — Identify talent pools and enrich candidate profiles instantly.
- **Market Researchers** — Map out competitive landscapes and track company growth metrics.


## Available Tools
- **add_monitor_target**: Add a target to an existing monitor feed
- **check_disposable_email**: Detect temporary or throwaway email addresses
- **get_company_details**: Retrieve comprehensive company metadata and leadership teams
- **get_company_employee_count**: Retrieve the estimated headcount range for a company
- **get_company_funding**: It may take up to 5 minutes.

Retrieve full funding history, rounds, and participating investors
- **get_company_logo**: Retrieve a 128x128 PNG logo URL for any company
- **get_company_updates**: Aggregate blog posts and X/Twitter updates into a mixed timeline
- **company_website_lookup**: Resolve a company name to its canonical website URL
- **get_competitor_listing**: Find competitors and the reasoning (keyword overlap or product similarity)
- **create_monitor_feed**: Create a new monitor feed for company changes
- **get_customer_listing**: Get a list of probable customers, investors, and partner platforms
- **get_employee_profile**: Enrich professional profiles from work emails or name/employer combinations
- **get_credit_balance**: Check your remaining API credit balance
- **get_monitor_rss**: Get the RSS feed for a specific monitor feed
- **list_monitor_feeds**: List all active monitor feeds
- **lookup_work_email**: Best-effort lookup of a public work email from a name and domain
- **search_employees**: Find current employees of a company by role and geography
- **get_similar_employees**: Repeat queries are served free from cache.

Find counterparts in similar roles at competing companies


## Installation & Usage

To install and use the **Proxycurl (LinkedIn Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/proxycurl-linkedin-data](https://vinkius.com/mcp/proxycurl-linkedin-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
