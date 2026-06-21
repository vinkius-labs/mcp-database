# Charity Navigator MCP Server

Search and evaluate US nonprofits — get charity ratings, financial health, advisories and cause data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/charity-navigator)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Connect to **Charity Navigator** and access ratings for over 175,000 US nonprofits through natural conversation.

### What you can do

- **Charity Search** — Search nonprofits by name, keyword, location, cause area or rating
- **Ratings** — Get Charity Navigator's overall rating (0-4 stars) plus financial health and accountability scores
- **Organization Details** — View mission statements, financials, website, contact info and tax filings
- **Rating History** — See how a charity's rating has changed over time
- **Advisories** — Check for warnings and alerts about charities with governance or financial concerns
- **Categories** — Browse charity categories and causes (education, health, environment, animal welfare, etc.)

### How it works

1. Subscribe to this server
2. Enter your Charity Navigator App ID and App Key (free registration)
3. Start evaluating charities from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Donors** — research charities before donating and verify their financial health
- **Researchers** — explore nonprofit ratings, financial data and governance records
- **Philanthropists** — search by cause area, location and rating to find vetted organizations


## Available Tools
- **get_all_advisories**: Useful for identifying charities with governance, financial or operational concerns.

Get all organizations with active advisories
- **get_categories**: Each category includes its ID, name, parent category and description. Use category IDs to filter charity searches by cause area (e.g. education, health, environment, animal welfare).

Get all charity categories and causes
- **get_charity**: Returns the charity name, EIN, mission statement, website, address, phone, financial data, tax filings and contact info. Use search_charities to find EINs.

Get detailed info for a specific charity by EIN
- **get_charity_advisories**: Advisories may include issues with financial management, governance or fundraising practices. Optionally filter by status (ALL, ACTIVE, REMOVED).

Get advisories/warnings for a specific charity
- **get_charity_ratings**: Returns all historical Charity Navigator ratings with overall score, financial health, accountability, transparency and impact scores. Shows how the charity's rating has changed over time.

Get rating history for a specific charity
- **search_charities**: Supports powerful filters: free-text search, state, city, zip code, rating (0-4 scale), category/cause, organization size by expenses, and whether the org is rated. Sort by rating, name or relevance. Pagination with pageSize (max 1000) and pageNum (max 10). Returns charity names, EIN, mission, ratings and financial info.

Search for charities and nonprofits by name, location or keyword


## Installation & Usage

To install and use the **Charity Navigator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/charity-navigator](https://vinkius.com/mcp/charity-navigator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
