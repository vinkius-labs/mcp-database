# Sproof MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sproof)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage digital signatures, documents, and contacts on Sproof with AI agents.

## Description
Connect your **Sproof** account to any AI agent to automate your European-compliant digital signature workflows. Sproof provides a premier platform for qualified electronic signatures (QES), and this integration allows you to retrieve document metadata, monitor signature requests, and manage contacts through natural conversation.

### What you can do

- **Document Orchestration** — List all managed documents and retrieve detailed profile metadata, including signature status programmatically.
- **Signature Request Control** — Create and monitor signature requests to ensure your legal documents are executed efficiently directly from the AI interface.
- **Contact Management** — Access and monitor your contact database to keep your signer records synchronized via natural language.
- **Profile & Account Oversight** — Retrieve detailed account profile metadata and monitor system usage to ensure your signature pipeline is optimized.
- **Compliance Monitoring** — Track document validity and signature authenticity using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Sproof API Key from your account settings
3. Start managing your digital signatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & Compliance Officers** — quickly retrieve document statuses and monitor signature requests without switching apps.
- **HR Managers** — automate the sending of employment contracts for signature via natural conversation.
- **Administrative Leads** — streamline the management of signed documents and monitor contact metadata directly within the chat.


## Available Tools
- **cancel_signature_request**: Cancel a pending signature request
- **create_contact**: Create a new contact for signing
- **create_signature_request**: Pass data as a JSON string.

Create a new signature request
- **get_document**: Get document details
- **get_profile**: Get account profile details
- **get_signature_request**: Get details for a signature request
- **list_audit_trail**: Get the audit trail for a signature request
- **list_contacts**: List all contacts
- **list_documents**: List all documents
- **list_signature_requests**: List all signature requests
- **list_signers**: List all signers for a signature request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sproof** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending signature requests in Sproof."

**🤖 AI Agent:**
> I've retrieved your requests. You have 3 pending documents: 'Consulting Agreement', 'Employee Handbook', and 'Vendor Terms'. Would you like to check who still needs to sign them?

---

**👤 You:**
> "Show me all pending signature requests with their signing progress and deadline status."

**🤖 AI Agent:**
> 12 pending signature requests. Urgent (3): "Service Agreement - Meridian" (2/4 signed, deadline tomorrow), "NDA - TechVentures" (0/2 signed, overdue 2 days), "Employment Contract - D. Kim" (1/1 signed, awaiting notarization). In Progress (5): avg 60% completion, deadlines within 2 weeks. Awaiting Review (4): documents uploaded, not yet sent. Total documents pending: 34 pages across 12 requests. Reminders sent today: 5 (auto). Average signing time: 1.4 days. Completion rate this month: 89%.

---

**👤 You:**
> "Create a new signature request for the annual vendor agreement and add three signers."

**🤖 AI Agent:**
> Signature request created: "Annual Vendor Agreement 2025-2026". Document: vendor_agreement_2025.pdf (12 pages). Signers added: 1) David Chen (Vendor, CEO) - david@vendor.com, 2) Sarah Williams (Procurement Manager) - sarah@yourcompany.com, 3) James Park (Legal Counsel) - james@yourcompany.com. Signing order: sequential (Vendor → Procurement → Legal). Signature fields placed: 6 (2 per signer). Deadline: June 1, 2025. Reminders: auto every 3 days. Audit trail: enabled. eIDAS qualified: yes. Invitation emails sent to all signers.


## ❓ FAQ

**Q: How do I find my Sproof API Key?**
Log in to your Sproof account, navigate to **Account Settings** > **API**, and you will find your unique secret API Key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sproof](https://vinkius.com/mcp/sproof)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sproof** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sproof` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sproof** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sproof": {
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
