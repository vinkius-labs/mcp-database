# Superdocu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/superdocu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document collection and client onboarding with Superdocu and AI agents.

## Description
### What you can do
- List and track document requests in real-time.
- Create new contacts and initiate onboarding workflows.
- Approve or reject document submissions directly from your AI agent.
- Manage your document collection process with automated follow-ups.

### How it works
1. Get your Superdocu API Key from your account settings.
2. Enter your credentials in Vinkius platform.
3. Start chatting with your Superdocu agent to manage your onboarding.

### Who is it for?
- HR teams managing employee onboarding.
- Legal and compliance officers collecting KYC/AML documents.
- Real estate and financial services streamlining client documentation.


## Available Tools
- **approve_request**: Approve a document request
- **create_contact**: Create a new contact
- **create_request**: Create a new document request
- **get_contact**: Get details for a specific contact
- **get_document**: Get metadata for a specific document
- **get_me**: Get current user/account information
- **get_request**: Get details of a specific document request
- **list_contacts**: List all contacts
- **list_documents**: List all documents
- **list_requests**: List document requests in Superdocu
- **list_workflows**: List available document workflows
- **reject_request**: Reject a document request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Superdocu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active document requests in Superdocu."

**🤖 AI Agent:**
> I've found 5 active requests: 1. ID Check (ID: 101), 2. Proof of Address (ID: 102), etc.

---

**👤 You:**
> "Show me all document collection requests with their completion status and missing documents."

**🤖 AI Agent:**
> 18 active collection requests. Complete (8, 44%): all documents received and verified. In Progress (7, 39%): avg 72% documents received. Missing documents: "Meridian Corp Onboarding" (3 of 8: tax certificate, insurance proof, bank details). "TechVentures KYC" (1 of 5: passport copy). "DataFlow Compliance" (2 of 6: SOC 2 report, privacy policy). Not Started (3, 17%): invitation sent, no response. Auto-reminders sent: 12 this week. Average collection time: 4.2 days. Expiring soon: 2 requests (deadline in 3 days).

---

**👤 You:**
> "Create a new document collection request for the annual compliance audit with 10 required documents."

**🤖 AI Agent:**
> Collection request created: "Annual Compliance Audit 2025". 10 required documents: 1) Financial statements. 2) Tax returns. 3) Insurance certificates. 4) SOC 2 Type II report. 5) Privacy policy. 6) Data processing agreement. 7) Employee handbook. 8) Business continuity plan. 9) Vendor risk assessments. 10) IT security audit report. Recipient: compliance@meridiancorp.com. Deadline: June 30, 2025. Branded portal page generated. Auto-reminders: every 5 days. Upload validation: file type and size checks enabled. E-signature required on submission.


## ❓ FAQ

**Q: How do I create a new document request?**
You can use the create_request tool by providing a Contact ID and a Workflow ID.

**Q: Can I approve documents using the AI agent?**
Yes, use the approve_request tool with the specific Request ID to approve it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/superdocu](https://vinkius.com/mcp/superdocu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Superdocu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `superdocu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Superdocu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "superdocu": {
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
