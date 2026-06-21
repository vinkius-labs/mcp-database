# Evisort Contract Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evisort-contract-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/evisort-contract-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/evisort-contract-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Equip your AI agent to manage contract documents, track AI-extracted provisions, and monitor workflows via the Evisort API.

## Description
Integrate **Evisort**, the AI-powered contract management and intelligence platform, directly into your AI workflow. Manage your legal document library and folders, track AI-extracted provisions and key contract data, monitor approval workflows and expiration alerts, and oversee your entire contract lifecycle using natural language.

### What you can do

- **Contract Oversight** — List and retrieve detailed information, party names, and effective dates for all your legal documents.
- **AI Data Intelligence** — Monitor extracted provisions and clauses, resolving complex legal data into actionable insights via chat.
- **Workflow Management** — Access and monitor contract approval workflows, tracking current steps and active reviewers in real-time.
- **Legal Auditing** — Retrieve high-level summaries of contract volume, expiration alerts, and organizational legal health instantly.

### How it works

1. Connect the Evisort integration to your AI assistant.
2. Authorize using your Evisort REST API Key (found in your account settings).
3. Orchestrate your contract management and legal operations through intuitive conversation.

### Who is this for?

- **Legal & GC Teams** — Quickly check contract expiration dates and provision details on the go.
- **Procurement & Sales Ops** — Research active contract terms and approval statuses via chat during deal negotiations.
- **Compliance Teams** — Monitor organizational contract metadata and audit logs instantly.


## Available Tools
- **get_evisort_account_metadata**: Retrieve metadata and limits for your Evisort account
- **get_document_detailed_intelligence**: Get detailed settings and AI-extracted data for a specific contract
- **list_upcoming_contract_expirations**: Retrieve a list of contracts that are approaching their expiration date
- **quick_contract_portfolio_audit**: Retrieve a high-level summary of documents, workflows, and alerts
- **list_contract_documents**: List all contract documents in your Evisort account
- **list_previously_expired_contracts**: Identify contracts that have already reached their expiration date
- **list_document_library_folders**: List all folders and directories in your contract library
- **list_high_monetary_value_contracts**: Identify contracts with a monetary value above a specific threshold (mock logic)
- **list_contract_provisions**: List all AI-extracted provisions and clauses for a specific document
- **list_contract_workflows**: List all contract approval and review workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evisort Contract Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contracts expiring in the next 30 days."

**🤖 AI Agent:**
> I've found 5 contracts approaching expiration, including the 'SaaS Agreement with CloudStack' and 'Vendor Terms - Global Logistics'. Would you like to see the renewal provisions for CloudStack?

---

**👤 You:**
> "Show me the provisions for contract ID 'DOC-12345'."

**🤖 AI Agent:**
> For contract 'DOC-12345' (NDA with Wayne Corp), I've retrieved several provisions: 'Non-Disclosure' (Section 2.1), 'Term' (3 years), and 'Governing Law' (New York). Should I pull the extracted text for the Non-Disclosure clause?

---

**👤 You:**
> "What is the status of the 'Master Services Agreement' workflow?"

**🤖 AI Agent:**
> The 'Master Services Agreement' workflow is currently at the 'Legal Review' step (Step 3/5). It is assigned to 'Sarah Miller'. It has been pending for 2 days. Would you like to see the previous comments from the Finance team?


## Installation & Usage

To install and use the **Evisort Contract Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evisort-contract-intelligence](https://vinkius.com/mcp/evisort-contract-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
