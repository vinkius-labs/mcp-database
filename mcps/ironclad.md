# Ironclad MCP Server

Manage contracts, workflows, approvals, and counterparties via Ironclad CLM — launch, track, and search agreements directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ironclad)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Ironclad** account to any AI agent and manage your entire contract lifecycle through natural conversation.

### What you can do

- **Workflows** — List active contract workflows, check current step, and track progress through review, approval, and signature
- **Launch Contracts** — Start new NDAs, MSAs, SOWs, or any contract type from pre-built templates with counterparty details
- **Records** — Search and browse the executed contract repository with key dates, values, and renewal terms
- **Approvals** — Check who approved, who is pending, and unblock stuck contracts
- **Templates** — Browse available contract types ready to launch
- **Comments** — Review internal discussion threads and negotiation notes on any contract

### How it works

1. Subscribe and enter your Ironclad API token (from **Company Settings → API → Access Tokens**)
2. Your AI agent connects to your Ironclad workspace
3. Ask questions like "show me pending contracts" or "launch an NDA for Acme Corp"

### Who is this for?

- **Legal Teams** — Track contract status, approvals, and negotiations without switching tabs
- **Sales Operations** — Launch contracts from templates and monitor deal velocity through legal review
- **Procurement Teams** — Manage vendor agreements, renewals, and compliance from conversation


## Available Tools
- **ironclad_get_approvals**: Returns each approver with their status (approved/pending/rejected), approval date, and any comments. Essential for tracking where a contract is stuck in the approval process. Use when the user asks "who still needs to approve this contract?" or "why is this contract delayed?"

Get the approval status of a specific Ironclad contract workflow — who approved, who is pending, and who rejected
- **ironclad_get_comments**: Returns each comment with author, timestamp, and message. Comments capture internal review discussions, legal feedback, and negotiation notes. Use to review the discussion history of a contract or understand decision context.

Get all comments and discussion on an Ironclad contract workflow — internal team communication and negotiation notes
- **ironclad_get_record**: Use for contract lookups, renewal planning, or compliance reviews.

Get complete details of an executed Ironclad contract record — all metadata, dates, obligations, and linked documents
- **ironclad_get_workflow**: ), current workflow step, assigned reviewers and approvers, counterparty name, related document links, and complete timeline of actions. Use to drill into a specific contract for status updates or details.

Get full details of a specific Ironclad contract workflow — current step, all attributes, counterparty info, and timeline
- **ironclad_launch_workflow**: Attributes is a JSON object containing the contract-specific fields defined in the template (e.g., counterparty name, contract value, effective date, jurisdiction). The workflow immediately enters the first step (typically internal review or drafting).

Launch a new Ironclad contract workflow from a template — start the process for an NDA, MSA, SOW, or any configured contract type
- **ironclad_list_records**: Returns contract name, counterparty, contract type, key dates (effective, expiration, renewal), total value, and status. Records are the final, executed versions of contracts. Use when the user asks about existing agreements, upcoming renewals, or the contract repository.

List executed contract records in Ironclad — fully signed agreements stored in the contract repository with key metadata
- **ironclad_list_templates**: Each template defines: the contract type (NDA, MSA, SOW, amendments, etc.), required attributes/fields, approval chain, and signature requirements. Template IDs are needed to launch new workflows via ironclad_launch_workflow. Use when the user asks "what contract types can we create?" or needs a template ID.

List available Ironclad workflow templates — NDA, MSA, SOW, and other pre-configured contract types ready to launch
- **ironclad_list_webhooks**: Webhooks are used to notify external systems when events occur in Ironclad (e.g., workflow launched, contract signed). Returns webhook ID, name, target URL, and events. Use when auditing integrations or checking connectivity.

List all configured webhooks in Ironclad — monitor external notifications for workflow events
- **ironclad_list_workflows**: Each workflow represents a contract moving through its lifecycle: drafting → internal review → approval → counterparty negotiation → signature → execution. Returns workflow name, current step/status, creator, counterparty, template used, and dates. Use when the user asks about contracts in progress, pending approvals, or the contract pipeline.

List Ironclad contract workflows in progress — NDAs, MSAs, SOWs, and other agreements moving through approval and signature stages
- **ironclad_search_records**: Matches contract names, counterparty names, descriptions, and attribute values. Use when the user asks "find our contract with Acme", "show all NDAs", or needs to locate a specific agreement by keyword.

Search Ironclad contract records by keyword — find specific agreements, counterparties, or contract types across the repository


## Installation & Usage

To install and use the **Ironclad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ironclad](https://vinkius.com/mcp/ironclad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
