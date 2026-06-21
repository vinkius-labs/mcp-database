# OpenLaws MCP Server

Access validated legal data via OpenLaws — search statutes, regulations, case law, validate citations, and track legislative changes directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openlaws)

## Overview
**Category:** brain-trust
**Tools Count:** 14

## Description
Connect your **OpenLaws** API account to any AI agent and take full control of legal research, citation validation, and legislative monitoring workflows through natural conversation.

### What you can do

- **Statute Search** — Search federal and state statutes by keyword (BM25) across all 50 states simultaneously, or scope to specific jurisdictions
- **Regulation Search** — Query Code of Federal Regulations (CFR) and state regulations with fast keyword search and jurisdiction filtering
- **Case Law Search** — Search ~5-6 million case opinions from Harvard CAP and CourtListener, filtered by jurisdiction, court, or federal circuit
- **Citation Validation** — Validate and identify malformed legal citations, find original government sources for citations across 53 jurisdictions
- **Constitutional Provisions** — Search US Constitution and all 50 state constitutions for specific provisions and amendments
- **Legislative History** — Retrieve historical versions of federal statutes and generate redline comparisons between legislative sessions
- **Recent Updates** — Monitor recent legal updates and changes across jurisdictions for compliance tracking

### How it works

1. Subscribe to this server
2. Enter your OpenLaws API Bearer token
3. Start researching laws, validating citations, and monitoring legislative changes from Claude, Cursor, or any MCP-compatible client

No more manual legal research across fragmented government websites. Your AI acts as a dedicated legal research assistant or compliance analyst.

### Who is this for?

- **Legal Professionals** — instantly search statutes, regulations, and case law across multiple jurisdictions without opening dozens of government websites
- **Compliance Teams** — monitor recent legislative updates and track regulatory changes to maintain compliance programs
- **LegalTech Developers** — integrate validated legal data into RAG pipelines, agentic workflows, and NLP/ML applications
- **Policy Researchers** — conduct 50-state surveys, analyze legislative history, and compare statutory changes over time


## Available Tools
- **get_caselaw_opinion**: Use this to get the complete court opinion after finding it via search_caselaw.
The response includes the full opinion text, court details, date, citations, and parties involved.

Get a specific case law opinion by its ID
- **get_constitution**: Use this to get the complete provision content after finding it via search_constitutions.
The response includes rich text content, article/section information, and amendments history.

Get a specific constitution provision by its ID
- **get_jurisdiction**: Use the jurisdiction_id from list_jurisdictions to inspect details before scoping searches.

Get details of a specific jurisdiction
- **get_recent_updates**: You can view updates across all jurisdictions or filter to a specific state/federal level.
This is useful for compliance monitoring and staying current with legislative changes.
Optionally specify jurisdiction ID and limit the number of results.
Example: check what changed in California employment law this month, or monitor federal regulatory updates.

Get recent legal updates across jurisdictions or in a specific jurisdiction
- **get_redline_comparison**: This shows exactly what changed between legislative sessions or amendment cycles.
Currently available for federal laws only (USC).
Optionally specify from and to version dates. If not specified, compares the two most recent versions.
Use this to understand legislative changes and their impact on compliance requirements.

Get redline comparison between two versions of a federal statute
- **get_regulation**: Use this to get the complete regulation content after finding it via search_regulations.
The response includes rich text content, citations, and regulatory context.

Get a specific regulation by its ID
- **get_statute_history**: This allows you to see how the law has changed over time.
Currently available for federal laws only (USC - United States Code).
Use the statute_id from search_statutes to view the legislative history and amendments.

Get historical versions of a federal statute
- **get_statute**: Use this to get the complete statute content after finding it via search_statutes.
The response includes rich text content, citations, effective dates, and annotations.

Get a specific statute by its ID
- **list_jurisdictions**: Jurisdictions include federal (US), all 50 states, District of Columbia, and Puerto Rico.
Each jurisdiction has an ID that can be used to scope searches to specific regions.
Use this to discover what jurisdictions are available before searching statutes, regulations, or caselaw.

List all available legal jurisdictions in OpenLaws
- **search_caselaw**: Data sourced from Harvard CAP project and CourtListener (~5-6 million cases).
You can filter by jurisdiction, specific court, or federal circuit.
The query parameter is required. Optionally filter by jurisdiction_id and court name.
Results include case opinions, court information, dates, and citations.
Example: search for " Fourth Amendment privacy" or "breach of contract" cases.

Search case law opinions by keyword
- **search_constitutions**: You can search the US Constitution and all 50 state constitutions simultaneously.
The query parameter is required. Optionally filter by jurisdiction ID.
Results include constitutional provisions, amendments, and relevant sections.
Example: search for "free speech" or "right to privacy" across all constitutions.

Search constitutions by keyword across jurisdictions
- **search_regulations**: You can search all jurisdictions simultaneously or scope to a specific region.
The query parameter is required and contains the search term. Optionally filter by jurisdiction ID.
Results include regulation text, citations, and contextual information.
Example: search for "environmental protection" or "workplace safety" regulations.

Search regulations by keyword across jurisdictions
- **search_statutes**: You can search all 50 states simultaneously for 50-state surveys, or scope to a specific jurisdiction.
The query parameter is required and contains the search term. Optionally filter by jurisdiction ID.
Results include statute text, citations, effective dates, and jurisdiction information.
Example: search for "data privacy" across all jurisdictions, or "employment" in California only.

Search statutes by keyword across jurisdictions
- **validate_citation**: This tool helps identify malformed citations and find the authoritative source document.
Supports citations from all 50 states, DC, Puerto Rico, and federal sources.
The citation parameter should be a standard legal citation format (e.g., "42 U.S.C. § 1983", "Brown v. Board of Education, 347 U.S. 483").
Use this to validate citations in legal documents, spreadsheets, or databases before relying on them.

Validate a legal citation and find its original source


## Installation & Usage

To install and use the **OpenLaws** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openlaws](https://vinkius.com/mcp/openlaws)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
