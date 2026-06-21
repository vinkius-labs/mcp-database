# OpenLaws MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openlaws)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Access validated legal data via OpenLaws — search statutes, regulations, case law, validate citations, and track legislative changes directly from any AI agent.

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


## Available Tools (14)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenLaws** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for data privacy statutes across all US states and summarize the key findings."

**🤖 AI Agent:**
> I've searched statutes for 'data privacy' across all 53 jurisdictions. Found relevant statutes in 12 states including California Consumer Privacy Act (CCPA), Virginia Consumer Data Protection Act, Colorado Privacy Act, and Connecticut Data Privacy Act. Federal: no comprehensive federal data privacy statute currently exists. Top results include: CA Civ. Code § 1798.100, Va. Code § 59.1-575, Colo. Rev. Stat. § 6-1-1303. Would you like the full text of any specific statute?

---

**👤 You:**
> "Validate these citations: '42 U.S.C. § 1983' and 'Roe v. Wade, 410 U.S. 113' and tell me if they're correct."

**🤖 AI Agent:**
> I've validated both citations:

1. **42 U.S.C. § 1983** — ✅ VALID. Civil Rights Act, Section 1983 (Deprivation of rights under color of law). Federal statute. Source: USC Title 42, Chapter 21, Subchapter 1.

2. **Roe v. Wade, 410 U.S. 113 (1973)** — ✅ VALID. Supreme Court opinion. Citation confirmed: 410 United States Reports 113. Note: Overturned by Dobbs v. Jackson Women's Health Organization (2022). Original source: Supreme Court of the United States.

Both citations are correctly formatted and verified against government sources.

---

**👤 You:**
> "Show me recent legislative updates in California employment law and any changes this month."

**🤖 AI Agent:**
> I've retrieved recent updates for California jurisdiction. Found 8 recent updates in the past 30 days:

1. **CA Labor Code § 2810.5** — Updated notice requirements for new hires (effective 2024-01-01)
2. **CA Labor Code § 432.7** — Amendments to salary history ban provisions
3. **CA Gov. Code § 12950.1** — Expanded SB-551 training requirements for employers with 50+ employees
4. **CA Code of Regs. tit. 8, § 11040** — Updated wage order exemptions for professional workers
5. **AB 1234 (2024)** — New remote work expense reimbursement requirements

Would you like the full text of any of these updates, or shall I search for specific topics like 'remote work' or 'overtime'?


## ❓ FAQ

**Q: How do I get an OpenLaws API key and what authentication method is used?**
Visit [**openlaws.us/api**](https://openlaws.us/api/) and click **Get API Access** to register. Once approved, you'll receive a Bearer token. Include it in the Authorization header as `Authorization: Bearer YOUR_TOKEN`. The API uses standard Bearer token authentication for all v1 endpoints at `https://api.openlaws.us/api/v1/`.

**Q: Can I search statutes across all 50 states simultaneously?**
Yes! Use the `search_statutes` tool without specifying a jurisdiction parameter to search all 53 jurisdictions (50 states + DC + Puerto Rico + federal) at once. This is perfect for 50-state surveys. Alternatively, scope your search to a specific jurisdiction by providing its ID (e.g., 'ca' for California, 'ny' for New York, 'us' for federal).

**Q: How does citation validation work and what formats are supported?**
Use the `validate_citation` tool with any standard legal citation format. The API will identify the original government source, validate the citation accuracy, and flag malformed citations. It supports Bluebook format (e.g., '42 U.S.C. § 1983', '347 U.S. 483 (Brown v. Board)'), state citations for all 50 states, DC, and Puerto Rico. This is ideal for validating citations in legal documents, spreadsheets, and databases.

**Q: What legal data sources does OpenLaws cover?**
OpenLaws covers ~4.3 million tracked sections across 53 jurisdictions with 100% federal statutes and regulations coverage. Data includes: United States Code (USC), Code of Federal Regulations (CFR), all 50 state statutes and regulations, DC and Puerto Rico laws, ~5-6 million case opinions (from Harvard CAP and CourtListener), US Constitution and all 50 state constitutions, and legislative history for federal laws.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openlaws](https://vinkius.com/mcp/openlaws)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenLaws** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openlaws` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenLaws** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openlaws": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
