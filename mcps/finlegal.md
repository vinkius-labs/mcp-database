# FinLegal MCP Server

Manage litigation funding cases, track claim progress, and coordinate legal finance workflows for law firms and funders.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/finlegal)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **FinLegal** account to any AI agent and take full control of your legal claims management and case orchestration through natural conversation.

### What you can do

- **Claim Orchestration** — List and manage legal claims programmatically, including retrieving detailed status updates and technical metadata across UK, US, and AU regions
- **Claimant CRM** — Manage complete profiles for contacts and claimants to maintain a high-fidelity database for your legal operations
- **Workflow Automation** — Programmatically create and track workflow activities (steps/forms) to ensure case progression and deadline adherence
- **Template Intelligence** — Access activity and attribute templates to understand valid data types and required steps for every claim type
- **Case Navigation** — Manage complex legal cases that act as containers for multiple individual claims to streamline high-volume legal management

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your FinLegal/CaseFunnel dashboard (Settings > API Keys)
3. Specify your **Region** (uk, us, or au) in the configuration
4. Start managing your legal operations from Claude, Cursor, or any MCP client

No more manual status checking or complex form navigation in the legal portal. Your AI acts as your dedicated legal operations and case coordinator.

### Who is this for?

- **Law Firms & Attorneys** — instantly check claim statuses and update case activities using natural language commands
- **Claim Management Companies** — automate claimant onboarding and monitor large-scale legal portfolios without leaving your workspace
- **Legal Ops Leads** — manage contact directories and verify workflow templates through simple AI queries


## Available Tools
- **create_activity**: Requires either claimId or contactId along with activityTemplateId.

Create or back-fill an activity (step/form) for a claim or contact
- **create_claim**: Create a new legal claim for a contact
- **create_contact**: Use isAdministrator=true for claim managers.

Create a new contact (Claimant or Admin)
- **get_case**: Get details for a specific case
- **get_claim**: Get details for a specific claim
- **get_contact_by_email**: Find a contact by their email address
- **get_contact**: Get details for a specific contact
- **list_activities**: List activities associated with a claim
- **list_activity_templates**: List available activity templates
- **list_attribute_templates**: List available attribute templates
- **list_claims**: List all claims
- **update_contact**: Update an existing contact


## Installation & Usage

To install and use the **FinLegal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finlegal](https://vinkius.com/mcp/finlegal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
