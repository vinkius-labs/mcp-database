# Bloomberg Law MCP Server

Access 200M+ court dockets, case law, and legal news via Bloomberg Law Enterprise Dockets API for comprehensive legal research.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bloomberg-law)

## Overview
**Category:** industry-titans
**Tools Count:** 13

## Description
Connect to **Bloomberg Law Enterprise Dockets API** and access 200 million+ federal and state court records, comprehensive case law database, and Bloomberg Law legal news—all from any AI agent. Search dockets, review filings, track litigation, and stay current on legal developments.

### What you can do

- **Docket Search** — Search 200M+ federal and state court dockets by party name, case name, docket number, or keywords
- **Federal Dockets** — Access District Courts, Circuit Courts of Appeals, Bankruptcy Courts, and Supreme Court dockets
- **State Dockets** — Search state court dockets across multiple jurisdictions (coverage varies by state)
- **Docket Details** — Get complete case information including parties, attorneys, judges, and status
- **Docket Entries** — View all filings, motions, and orders for any docket with timestamps and descriptions
- **Filing Documents** — Access full text of court filings and documents
- **Case Law Search** — Search Bloomberg Law's comprehensive case law database for precedents and holdings
- **Legal News** — Search and browse Bloomberg Law's legal news articles, analysis, and commentary
- **Expert Witnesses** — Find expert witnesses by specialty, prior testimony, and jurisdiction
- **Company Profiles** — Search company business intelligence and legal exposure data
- **Docket Alerts** — View configured alerts monitoring specific cases, parties, or keywords

### How it works

1. Subscribe to this server
2. Enter your Bloomberg Law Enterprise API key (requires Bloomberg Law subscription)
3. Start researching court dockets, cases, and legal news from Claude, Cursor, or any MCP-compatible client

Your AI becomes a legal research assistant, helping you find cases, track dockets, and stay current on legal developments.

### Who is this for?

- **Litigators** — search dockets, track opposing party litigation, and monitor case developments
- **Corporate Counsel** — track litigation involving your company, competitors, and key business partners
- **Legal Researchers** — access case law, precedents, and holdings for legal analysis
- **Journalists** — stay current on legal news and find court cases for reporting
- **Paralegals** — quickly find dockets, filings, and case details across jurisdictions
- **Academics** — research litigation trends, case outcomes, and legal developments


## Available Tools
- **get_case_details**: Get detailed information for a specific legal case
- **get_docket_alerts**: Get configured docket alerts for monitoring cases
- **get_docket_details**: Use docket ID from search results.

Get detailed information for a specific court docket
- **get_docket_entries**: Each entry includes entry number, filing date, description, and document links.

Get all entries/filings for a specific court docket
- **get_filing_document**: Use document ID from docket entries results.

Get a specific filing document from a court docket
- **get_legal_news_by_topic**: Get legal news articles by specific topic
- **search_legal_cases**: Returns case summaries, holdings, and outcomes. Filter by jurisdiction and date for precedent analysis.

Search for legal cases and case law
- **search_companies**: Search company profiles and business intelligence
- **search_court_dockets**: Returns docket numbers, case names, courts, filing dates, and status. Filter by court, date range, and keywords.

Search federal and state court dockets across 200M+ case records
- **search_expert_witnesses**: Find experts by specialty, prior testimony, and jurisdiction.

Search for expert witnesses in litigation
- **search_federal_dockets**: Search federal court dockets specifically
- **search_legal_news**: Filter by topic and date range.

Search Bloomberg Law legal news articles
- **search_state_dockets**: Coverage varies by state.

Search state court dockets


## Installation & Usage

To install and use the **Bloomberg Law** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bloomberg-law](https://vinkius.com/mcp/bloomberg-law)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
