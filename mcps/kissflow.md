# Kissflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kissflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build low-code workflows, process apps, and case management solutions that digitize operations without heavy IT involvement.

## Description
Connect your **Kissflow** account to any AI agent and manage workflows through natural conversation.

### What you can do

- **Process Management** — List and inspect automated workflows and processes
- **Request Tracking** — Browse, create, and update requests within processes
- **Form Access** — View form fields and data schemas for each process
- **Approval Monitoring** — Track pending approvals and their status
- **Data Access** — Query process data with filters and pagination

### How it works

1. Subscribe to this server
2. Enter your Kissflow Access Key ID, Secret Access Key, Subdomain, and Account ID
3. Start managing workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations** — manage automated workflows and track requests
- **Managers** — monitor approvals and process bottlenecks
- **IT Teams** — access process data and configuration


## Available Tools (9)
- **get_user_details**: Essential for reviewing detailed profile information.

Get details for a specific user
- **list_dataform_items**: Use this to export or review collected form data.

List entries within a dataform
- **list_dataforms**: Dataforms are used for data collection without complex workflow logic.

List all dataforms
- **list_dataset_items**: Essential for querying master data or reference tables.

List records within a dataset
- **list_datasets**: Datasets serve as central tables for master data management.

List all datasets
- **list_groups**: Useful for managing access control.

List user groups
- **list_process_items**: Useful for tracking the progress of individual flow requests.

List items within a process
- **list_processes**: Processes are used to manage multi-step business logic.

List all workflow processes
- **list_users**: Use this to identify user IDs and email addresses.

List all Kissflow users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kissflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all processes and pending approvals across workflows."

**🤖 AI Agent:**
> Processes: 8. Purchase Request (45 active), Leave Approval (12), Expense Report (23), IT Request (8), Onboarding (3), Travel Request (6), Budget Approval (2), Vendor Registration (4). Pending approvals: 14 total. Critical: 'Server Purchase — $25K' (Budget, awaiting CFO, 3 days). 'Q2 Marketing Budget — $50K' (Budget, VP pending).

---

**👤 You:**
> "Create a new purchase request and list recent expense reports."

**🤖 AI Agent:**
> Purchase request created! 'New Developer Laptops (5x MacBook Pro)' — Amount: $12,500. Department: Engineering. Justification: Team expansion. Status: Pending Manager Approval. Recent expense reports: 12 this month. Total: $8,400. Pending reimbursement: $3,200. Top: 'Client Dinner' ($450), 'Conference Travel' ($1,800).

---

**👤 You:**
> "Show the form fields for Leave Approval and all active leave requests."

**🤖 AI Agent:**
> Leave Approval fields: 6. Employee Name (auto, required), Leave Type (dropdown: Vacation, Sick, Personal, Bereavement), Start Date (date), End Date (date), Reason (textarea), Backup Person (dropdown). Active requests: 12. Vacation: 7, Sick: 3, Personal: 2. Pending approval: 4. Approved: 6. Rejected: 2.


## ❓ FAQ

**Q: Can I create and track requests within processes?**
Yes. Create new requests within any process, update request data, and track them through workflow stages including pending approvals.

**Q: Does Kissflow require four credentials?**
Yes. Kissflow requires **Access Key ID**, **Secret Access Key**, **Subdomain**, and **Account ID**. Requests go to `https://{subdomain}.kissflow.com/v1/{accountId}/`.

**Q: Can I monitor pending approvals?**
Yes. Track all pending approvals across processes with assignee, status, and deadline information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kissflow](https://vinkius.com/mcp/kissflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kissflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kissflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kissflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kissflow": {
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
