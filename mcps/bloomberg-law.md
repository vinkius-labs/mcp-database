# Bloomberg Law MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bloomberg-law)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bloomberg-law-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bloomberg-law-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access 200M+ court dockets, case law, and legal news via Bloomberg Law Enterprise Dockets API for comprehensive legal research.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bloomberg Law** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for dockets involving Apple Inc in federal courts."

**🤖 AI Agent:**
> Found 23 federal dockets involving Apple Inc. Recent cases include: 1) Apple Inc v. Epic Games (NDCA, 1:20-cv-05583) — ongoing antitrust litigation, 2) Apple Inc v. Corellium (SDFL, 9:19-cv-81124) — copyright dispute, 3) In re: Apple iPhone Antitrust Litigation (NDCA, consolidated) — class action. Would you like to see docket entries for any of these cases?

---

**👤 You:**
> "Show me the latest legal news on data privacy regulation."

**🤖 AI Agent:**
> Found 8 recent articles on data privacy regulation: 1) "Supreme Court to Hear Major Privacy Case on Third-Party Doctrine" (April 7, 2026), 2) "EU-US Data Privacy Framework Faces New Legal Challenge" (April 6, 2026), 3) "California Expands Consumer Privacy Rights Under CPRA" (April 5, 2026), 4) "FTC Announces New Privacy Enforcement Priorities" (April 4, 2026).

---

**👤 You:**
> "Get the docket entries for case 1:24-cv-12345 in SDNY."

**🤖 AI Agent:**
> Found 47 docket entries for 1:24-cv-12345 (SDNY). Recent entries: 1) Entry 47 — Motion for Summary Judgment filed by Plaintiff (April 5, 2026), 2) Entry 46 — Defendant's Response to Discovery Requests (April 3, 2026), 3) Entry 45 — Court Order Setting Discovery Deadline (March 28, 2026), 4) Entry 44 — Joint Case Management Plan filed (March 15, 2026). Would you like to view the full text of any filing?


## Installation & Usage

To install and use the **Bloomberg Law** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bloomberg-law](https://vinkius.com/mcp/bloomberg-law)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
