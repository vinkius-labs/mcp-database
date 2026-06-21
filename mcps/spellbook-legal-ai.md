# Spellbook Legal AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spellbook-legal-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI-powered contract drafting and review — analyze contracts, draft clauses, detect risks, and compare against 2,000+ market precedents via Spellbook.

## Description
Connect to **Spellbook Legal AI** and bring AI-powered contract drafting, review, and analysis to any AI agent. Trusted by 4,000+ in-house teams and law firms worldwide, Spellbook helps transactional lawyers draft and review contracts faster and more accurately.

### What you can do

- **Contract Analysis** — AI-powered review of contracts identifying risks, missing clauses, non-standard terms, and issues
- **Clause Suggestions** — Get AI-generated clause suggestions based on market standards and best practices
- **Contract Comparison** — Compare two contract versions to identify additions, deletions, and modifications
- **Market Comparison** — Compare contract terms against 2,000+ market precedents showing pro-buyer, pro-seller, and market-standard positions
- **AI Clause Drafting** — Generate AI-drafted clauses based on specified requirements, jurisdiction, and party position
- **Contract Summarization** — Generate concise summaries highlighting key terms, obligations, and risks
- **Risk Assessment** — Get comprehensive risk assessments with high, medium, and low risk issues and remediations
- **Playbook Compliance** — Check contracts against company playbooks to identify deviations from standards
- **Clause Library Search** — Search Spellbook's extensive clause library for standard, market-tested clauses
- **Document Management** — Upload, list, and search contract documents with filtering by status and type

### How it works

1. Subscribe to this server
2. Enter your Spellbook API key (available in Spellbook account settings)
3. Start drafting and reviewing contracts from Claude, Cursor, or any MCP-compatible client

Your AI becomes a transactional legal assistant, helping you draft clauses, review contracts, identify risks, and ensure market-standard terms.

### Who is this for?

- **Transactional Lawyers** — draft and review contracts with AI-powered clause suggestions and market comparisons
- **In-House Legal Teams** — review vendor and customer contracts against company playbooks and standards
- **Contract Managers** — analyze contracts for risks, track changes between versions, and manage document libraries
- **Legal Operations** — automate contract review workflows and ensure consistent clause usage
- **Law Students** — practice contract drafting and learn market-standard clause positions


## Available Tools
- **analyze_spellbook_contract**: USE WHEN:
- User wants to review a contract for risks
- User needs to identify issues in a contract
- User asks to "analyze this contract" or "review for risks"

PARAMETERS:
- document_id (REQUIRED): ID of the document to analyze
- analysis_type (OPTIONAL): Type of analysis — "full" (default), "risks_only", "clause_check", "market_comparison"

EXAMPLES:
- "Analyze document 123 for risks" → call with document_id="123"
- "Review this contract for issues" → call with document_id="123", analysis_type="full"
- "Check clauses in document 456" → call with document_id="456", analysis_type="clause_check"

Analyze a contract document for risks, issues, and suggestions
- **check_spellbook_playbook**: Check contract compliance against a playbook
- **compare_spellbook_contracts**: USE WHEN:
- User wants to compare two versions of a contract
- User needs to identify changes between drafts
- User asks to "compare these contracts" or "show differences"

PARAMETERS:
- document_id_1 (REQUIRED): ID of the first document
- document_id_2 (REQUIRED): ID of the second document
- comparison_type (OPTIONAL): Type of comparison — "full" (default), "clauses_only", "risk_comparison"

EXAMPLES:
- "Compare documents 123 and 456" → call with document_id_1="123", document_id_2="456"
- "Show differences between contract versions" → call with document_id_1="123", document_id_2="456", comparison_type="full"

Compare two contract versions to identify differences
- **draft_spellbook_clause**: USE WHEN:
- User needs to draft a new clause for a contract
- User wants AI to generate standard clause language
- User asks to "draft a limitation of liability clause" or "write an indemnification clause"

PARAMETERS:
- clause_type (REQUIRED): Type of clause to draft (e.g. "Limitation of Liability", "Indemnification", "Confidentiality")
- party_position (OPTIONAL): Which party position to draft for — "neutral" (default), "pro-buyer", "pro-seller", "pro-vendor"
- jurisdiction (OPTIONAL): Jurisdiction for the clause (e.g. "New York", "Delaware", "California", "UK")
- custom_instructions (OPTIONAL): Additional instructions or requirements for the clause

EXAMPLES:
- "Draft a limitation of liability clause" → call with clause_type="Limitation of Liability"
- "Draft a pro-buyer indemnification clause for New York" → call with clause_type="Indemnification", party_position="pro-buyer", jurisdiction="New York"
- "Write a confidentiality clause with custom instructions" → call with clause_type="Confidentiality", custom_instructions="Include data breach notification requirements"

Draft a contract clause using Spellbook AI
- **get_spellbook_clause_suggestions**: Get AI clause suggestions for a contract document
- **get_spellbook_document**: Get detailed information for a specific contract document
- **get_spellbook_market_comparison**: Shows pro-buyer, pro-seller, and market-standard positions.

Get market comparison data for a specific clause type
- **get_spellbook_risk_assessment**: Get a detailed risk assessment for a contract document
- **list_spellbook_documents**: Supports filtering by status, document type, and date range.

USE WHEN:
- User wants to see all their contract documents
- User needs to find contracts by status or type
- User is exploring their document library
- User asks "what contracts do I have" or "list my documents"

PARAMETERS:
- status (OPTIONAL): Filter by document status (e.g. "Draft", "In Review", "Finalized")
- document_type (OPTIONAL): Filter by document type (e.g. "NDA", "MSA", "SOW", "Employment Agreement")
- date_from (OPTIONAL): Start date filter (YYYY-MM-DD)
- date_to (OPTIONAL): End date filter (YYYY-MM-DD)
- page (OPTIONAL): Page number for pagination
- page_size (OPTIONAL): Results per page (default: 25, max: 100)

EXAMPLES:
- "List all my contract documents" → call with no params
- "Show contracts in review" → call with status="In Review"
- "List NDAs" → call with document_type="NDA"

List all contract documents in Spellbook
- **search_spellbook_clause_library**: Search the Spellbook clause library for standard clauses
- **search_spellbook_documents**: Search contract documents by keyword
- **summarize_spellbook_contract**: Generate an AI summary of a contract document
- **upload_spellbook_document**: USE WHEN:
- User wants to upload a new contract for review
- User needs to analyze a contract received from another party
- User asks to "upload this contract" or "analyze this document"

PARAMETERS:
- file_name (REQUIRED): Name of the document file
- file_content (REQUIRED): Base64-encoded file content or document text
- document_type (OPTIONAL): Type of document (e.g. "NDA", "MSA", "SOW")

EXAMPLES:
- "Upload this NDA for review" → call with file_name="NDA.pdf", file_content="[base64 content]", document_type="NDA"
- "Analyze this MSA contract" → call with file_name="MSA.docx", file_content="[base64 content]", document_type="MSA"

Upload a contract document to Spellbook for analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spellbook Legal AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this NDA for risks and issues."

**🤖 AI Agent:**
> Contract analysis complete for 'NDA - Acme Corp.pdf'. Found 3 risks: 1) [High] Unlimited liability exposure — recommend adding mutual liability cap at $X, 2) [Medium] Missing return of confidential materials provision — add clause requiring return/destruction of materials upon termination, 3) [Low] Term is longer than market standard (5 years vs typical 2-3 years). Overall risk level: Medium-High.

---

**👤 You:**
> "Draft a pro-buyer limitation of liability clause for Delaware."

**🤖 AI Agent:**
> Clause drafted: 'Limitation of Liability. EXCEPT FOR BREACHES OF CONFIDENTIALITY OBLIGATIONS, INFRINGEMENT OF INTELLECTUAL PROPERTY RIGHTS, OR INDEMNIFICATION OBLIGATIONS, IN NO EVENT SHALL EITHER PARTY'S TOTAL AGGREGATE LIABILITY ARISING OUT OF OR RELATED TO THIS AGREEMENT EXCEED THE TOTAL AMOUNTS PAID BY BUYER TO SELLER IN THE TWELVE (12) MONTHS IMMEDIATELY PRECEDING THE EVENT GIVING RISE TO LIABILITY.' Jurisdiction: Delaware, Position: Pro-Buyer.

---

**👤 You:**
> "Compare the market standard for indemnification clauses."

**🤖 AI Agent:**
> Market Comparison for Indemnification: 1) Market Standard (65% of contracts): Mutual indemnification for IP infringement, confidentiality breaches, and third-party claims, 2) Pro-Buyer Position (20%): Seller indemnifies buyer for all claims arising from seller's performance, with no cap, 3) Pro-Seller Position (15%): Limited indemnification capped at fees paid in prior 12 months, excluding consequential damages. Your current clause aligns with Market Standard.


## ❓ FAQ

**Q: What types of contracts can Spellbook analyze?**
Spellbook can analyze a wide range of commercial contracts including NDAs, MSAs, SOWs, employment agreements, vendor agreements, customer contracts, licensing agreements, real estate contracts, and more. The AI is trained on thousands of market precedents and can identify risks, non-standard terms, and missing clauses across all common commercial contract types.

**Q: How does the market comparison feature work?**
The market comparison feature compares your contract clauses against 2,000+ market precedents to show how your terms compare to market standards. It shows pro-buyer, pro-seller, and market-standard positions for each clause type, helping you understand whether your terms are favorable, aggressive, or in line with market norms.

**Q: How do I get a Spellbook API key?**
Visit Spellbook.legal and sign up for an account. Navigate to Settings → Integrations or API Settings in your account dashboard to generate an API key. The key gives you access to contract analysis, clause drafting, risk detection, and market comparison features. Contact Spellbook support if you need help setting up API access.

**Q: Can Spellbook draft custom clauses for specific jurisdictions?**
Yes! When drafting clauses with `draft_spellbook_clause`, you can specify the jurisdiction (e.g. New York, Delaware, California, UK, EU), party position (pro-buyer, pro-seller, neutral), and custom instructions. The AI generates clauses tailored to the specified jurisdiction's legal requirements and your preferred negotiating position.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spellbook-legal-ai](https://vinkius.com/mcp/spellbook-legal-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spellbook Legal AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `spellbook-legal-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spellbook Legal AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spellbook-legal-ai": {
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
