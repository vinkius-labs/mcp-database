# Copilot CRM (Assembly) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copilot-crm-assembly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Equip your AI agent to manage clients, companies, invoices, and files directly within your Copilot (Assembly) portal.

## Description
Integrate **Copilot** (now rebranding to **Assembly**), the leading client portal and CRM platform for service businesses, directly into your AI workflow.

### What you can do

- **Client Management** — List, retrieve, and update client profiles and company associations.
- **Billing Automation** — Monitor invoices, check statuses, and pull payment details via chat.
- **Portal Discovery** — Search for files, messages, and custom fields within your client workspace.

### How it works

1. Connect the Copilot integration to your AI assistant.
2. Authorize using your Copilot API Key (found in Settings > API).
3. Manage your entire client back-office using natural language.

### Who is this for?

- **Agencies & Consultancies** — Streamline client onboarding and project tracking without leaving the chat.
- **Accountants & Law Firms** — Quickly check invoice statuses or pull client documents during planning.
- **Support Teams** — Retrieve client custom fields and portal messages to provide faster assistance.


## Available Tools (10)
- **create_client**: Creates a new client record with identity properties (name, email) and optional company linkages.

Create a new client in the portal
- **get_client_details**: Resolves granular profile data, including contact information, associated company linkages, and system-level metadata.

Get detailed information about a specific client
- **list_clients**: Resolves client identity properties including unique identifiers, names, emails, and account status across the portal system boundary.

List all clients in your Copilot CRM
- **list_companies**: Resolves corporate entity properties such as company IDs, legal names, and primary contact associations.

List all companies in your Copilot CRM
- **list_custom_fields**: Resolves custom field definitions, including field keys, data types, and display labels used across various entities.

Retrieve definitions for custom fields used in CRM
- **list_files**: Resolves file metadata including filenames, storage paths, upload timestamps, and access permissions.

List files uploaded to the Copilot portal
- **list_forms**: Resolves form definitions, including titles, submission endpoints, and configuration metadata.

List intake or feedback forms available
- **list_invoices**: Resolves billing data including amounts, due dates, payment status, and client/company bill-to associations.

List all invoices and their statuses
- **list_portal_messages**: Resolves portal message threads, including sender/receiver identity, message content summary, and timestamps.

List messages sent through the client portal
- **update_client**: Modifies specific attributes like name or account status while preserving other entity properties.

Update existing client details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copilot CRM (Assembly)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active clients in my CRM."

**🤖 AI Agent:**
> I found 15 active clients. Some of the most recent ones are 'Acme Corp', 'Global Logistics', and 'John Smith'. Would you like to see the contact details for any of them?

---

**👤 You:**
> "Check the status of my pending invoices."

**🤖 AI Agent:**
> You have 3 pending invoices totaling $4,500. Invoice #1024 for 'Beta Systems' is overdue by 5 days. Should I send a reminder?

---

**👤 You:**
> "Search for any files uploaded by 'Acme Corp'."

**🤖 AI Agent:**
> I found 2 files for 'Acme Corp': 'Q1-Report.pdf' and 'Contract-Signed.docx'. Would you like the links to download them?


## ❓ FAQ

**Q: How do I generate an API Key in Copilot?**
Log in to your Copilot (Assembly) dashboard. Go to **Settings > API** and click 'Generate API Key'. Copy the key and paste it below.

**Q: Can the agent see my internal portal messages?**
Yes, if granted access via the API Key, the agent can list and retrieve messages sent through the client portal to help you keep track of communications.

**Q: Is the billing data secure?**
Absolutely. This integration uses standard API protocols and does not store your payment information. It only retrieves statuses and metadata provided by the Copilot API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copilot-crm-assembly](https://vinkius.com/mcp/copilot-crm-assembly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copilot CRM (Assembly)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `copilot-crm-assembly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copilot CRM (Assembly)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copilot-crm-assembly": {
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
