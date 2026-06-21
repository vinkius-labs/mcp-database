# Guidewire ClaimCenter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidewire-claimcenter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guidewire-claimcenter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guidewire-claimcenter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage insurance claims via ClaimCenter — track claim status, monitor exposures, and manage activities directly from any AI agent.

## Description
Connect your **Guidewire ClaimCenter** account to any AI agent and take full control of your insurance claims management through natural conversation. Streamline how you monitor and update claims natively.

### What you can do

- **Claim Oversight** — List and retrieve details for all active and historical insurance claims natively
- **Exposure Intelligence** — Access and monitor exposures associated with specific claims flawlessly
- **Activity Management** — List and review current activities and tasks across all claims securely
- **Document & Note Auditing** — List internal notes and uploaded documents for any claim flawlessly
- **User & Contact Logistics** — Access internal user rosters and shared contacts, including claimants and vendors, securely
- **Workflow Visibility** — Retrieve detailed claim metadata, policy numbers, and status updates directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClaimCenter Cloud API Username, Password, and Instance URL
3. Start managing your insurance claims from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Claims Adjusters** — monitor claim status and review recent activities using natural language
- **Claims Managers** — audit exposure volumes and team task lists without opening the core application
- **Support Teams** — quickly look up claim details and policy references straight from their chat interface
- **Insurance Ops** — verify document uploads and note history during claim processing


## Available Tools
- **list_claim_activities**: List current activities and tasks across all claims
- **list_claimcenter_claims**: List insurance claims from Guidewire ClaimCenter
- **list_claim_contacts**: List shared contacts (claimants, vendors, providers)
- **list_claim_documents**: List uploaded documents for a specific claim
- **list_claim_exposures**: List exposures associated with a specific claim
- **list_claim_notes**: List internal notes for a specific claim
- **list_claimcenter_users**: List internal users and claim adjusters
- **get_claim_details**: Get detailed information for a specific claim


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guidewire ClaimCenter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all claims with a status of 'Open' in ClaimCenter."

**🤖 AI Agent:**
> Retrieving your open claims... I found 5 items: Claim #000-01-0001 (Auto), #000-01-0002 (Property), and 3 others. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the exposures for claim '000-01-0001'."

**🤖 AI Agent:**
> Checking exposures for claim 000-01-0001... There are 2 active exposures: 1 for 'Vehicle Damage' (Adjuster: John Doe) and 1 for 'Liability' (Adjuster: Jane Smith).

---

**👤 You:**
> "Who is the primary contact for claim '000-01-0002'?"

**🤖 AI Agent:**
> Retrieving contacts for claim 000-01-0002... The primary contact is Mark Miller (Claimant). I can provide his phone number or email if needed.


## Installation & Usage

To install and use the **Guidewire ClaimCenter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidewire-claimcenter](https://vinkius.com/mcp/guidewire-claimcenter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
