# Documo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/documo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/documo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/documo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage digital faxes, track fax numbers, and monitor transmissions via the Documo API.

## Description
Integrate **Documo**, the next-generation digital fax and document workflow platform (mFax), directly into your AI workflow. Manage your inbound and outbound faxes, track assigned fax numbers, monitor transmission logs and delivery receipts, and oversee user access using natural language.

### What you can do

- **Fax Oversight** — List and retrieve detailed information and delivery status for all your digital fax transmissions.
- **Line Management** — Access and monitor all fax numbers assigned to your Documo account and their associated users.
- **Transmission Intelligence** — Monitor real-time transmission logs, page counts, and secure delivery receipts via chat.
- **User Auditing** — List and retrieve profile information for all users registered in your Documo organization.

### How it works

1. Connect the Documo integration to your AI assistant.
2. Authorize using your Documo (mFax) API Key (found in your platform settings).
3. Orchestrate your digital fax operations and document workflows through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly check transmission statuses and fax volumes on the go.
- **Legal & Healthcare Admins** — Monitor inbound documents and delivery receipts via chat for compliance.
- **IT Administrators** — Audit assigned fax lines and user access permissions instantly.


## Available Tools
- **get_documo_account_metadata**: Retrieve metadata and usage limits for your Documo account
- **get_fax_details**: Get detailed information and status for a specific fax
- **quick_fax_volume_audit**: Retrieve a high-level summary of fax transmissions and success rates
- **list_failed_fax_deliveries**: Identify faxes that failed to transmit correctly (mock logic)
- **list_assigned_fax_numbers**: List all fax numbers assigned to your Documo account
- **list_digital_faxes**: List all digital faxes in your Documo/mFax account
- **list_received_digital_faxes**: Identify faxes that have been received by your organization
- **list_latest_fax_transmissions**: Identify the most recently sent or received faxes
- **list_documo_users**: List all users registered in your Documo organization
- **search_faxes_by_recipient**: Search for faxes matching a recipient number or identifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Documo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recently sent faxes."

**🤖 AI Agent:**
> I've found 5 recent transmissions, including faxes to '+1 (555) 0123' and '+1 (555) 9876'. All were successfully delivered. Would you like to see the page count for any of these?

---

**👤 You:**
> "Show me all fax numbers assigned to our account."

**🤖 AI Agent:**
> Your account has 3 active fax numbers: '+1 (555) 1111' (Main Office), '+1 (555) 2222' (HR), and '+1 (555) 3333' (Support). Should I check the inbound fax volume for any of these lines?

---

**👤 You:**
> "Check the status of fax 'FAX-9988'."

**🤖 AI Agent:**
> Fax 'FAX-9988' sent to '+1 (555) 4444' is currently 'Delivered'. It was 4 pages long and transmitted via the 'Main Office' line. Should I pull the delivery receipt?


## Installation & Usage

To install and use the **Documo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/documo](https://vinkius.com/mcp/documo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
