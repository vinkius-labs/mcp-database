# Adobe Acrobat Sign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adobe-acrobat-sign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send, track, and manage e-signatures via Adobe Acrobat Sign — create agreements, check signing status, and access audit trails from any AI agent.

## Description
Connect your **Adobe Acrobat Sign** account to any AI agent and manage your entire e-signature workflow through natural conversation.

### What you can do

- **Agreements** — List, search, create, and cancel e-signature agreements
- **Signing Status** — Track who has signed, who is pending, and send reminders to signers
- **Audit Trails** — Access legally binding audit trails for any signed agreement
- **Library Documents** — Browse reusable templates and library documents
- **Document Upload** — Upload documents for signature via the transient document workflow
- **Participants** — View all signers, approvers, and CC recipients with their status

### How it works

1. Subscribe and enter your Adobe Sign access token and base URL (from **Adobe Admin Console → Acrobat Sign → API**)
2. Your AI agent connects to your Adobe Sign account
3. Ask questions like "send this contract for signature" or "has the NDA been signed?"

### Who is this for?

- **Legal Departments** — Send contracts and NDAs for signature, track completion, and maintain audit trails
- **HR Teams** — Manage offer letters, onboarding documents, and policy acknowledgments
- **Procurement** — Get vendor agreements signed quickly and maintain compliance records


## Available Tools (10)
- **adobe_agreement_members**: Returns each member email, role (SIGNER/APPROVER/ACCEPTOR/FORM_FILLER/DELEGATE_TO_SIGNER/CC), and their signing status. Use to check who has signed, who is pending, or to review the signing workflow.

Get all participants (signers, approvers, CC recipients) in a specific Adobe Sign agreement with their roles and status
- **adobe_audit_trail**: The audit trail is a legally binding record of all actions taken: when the agreement was created, viewed, signed, and by whom (with IP addresses and timestamps). Essential for legal compliance and dispute resolution.

Get the legal audit trail for an Adobe Sign agreement — a tamper-proof record of all signing events and actions
- **adobe_cancel_agreement**: This is irreversible — the agreement cannot be re-sent (a new one must be created). An optional comment explains the cancellation reason to all participants. Use when a deal falls through, terms change, or the document needs to be replaced.

Cancel an Adobe Sign agreement that is currently out for signature — stops the signing process and notifies all parties
- **adobe_create_agreement**: Create a new Adobe Sign agreement and send it for signature — the core e-signature workflow for contracts, NDAs, and legal documents
- **adobe_get_agreement**: Returns name, status, all participant sets with their roles (SIGNER/APPROVER/CC/DELEGATE), signature type, creation and modification dates, and any external IDs. Use after listing agreements to drill into a specific agreement for complete information.

Get complete details of a specific Adobe Sign agreement by ID, including all participants, signing status, and document metadata
- **adobe_list_agreements**: Returns agreement name, current status, signature type (ESIGN/WRITTEN), creator email, and creation/modification dates. Agreement statuses: DRAFT (being built), OUT_FOR_SIGNATURE (awaiting signatures), SIGNED (fully executed), CANCELLED, EXPIRED. Use when the user asks about pending signatures, completed agreements, or document pipeline.

List Adobe Acrobat Sign agreements with name, status (DRAFT/OUT_FOR_SIGNATURE/SIGNED/CANCELLED/EXPIRED), sender, and dates
- **adobe_list_library_documents**: Library documents are reusable templates that can be referenced when creating new agreements. Returns document name, ID (for use in adobe_create_agreement fileInfos), sharing mode, and creation date. Use when the user asks "what templates do we have?" or needs a library document ID.

List reusable library documents (templates) in Adobe Sign — pre-built agreements, forms, and document templates
- **adobe_search_agreements**: Returns matching agreements with names, statuses, and dates. Use when the user wants to find a specific agreement, look up a contract by name, or search across the document library.

Search Adobe Sign agreements by name or keyword to find specific documents across your signature pipeline
- **adobe_send_reminder**: The agreement must be in OUT_FOR_SIGNATURE status. An optional comment is included in the reminder email. Use when the user says "remind them to sign" or "send a reminder for the contract."

Send a signing reminder to all pending signers on an Adobe Sign agreement — nudges recipients who have not yet signed
- **adobe_upload_document**: Returns a transientDocumentId that is then used in adobe_create_agreement fileInfos. This is the standard workflow: (1) upload document → (2) create agreement with the transientDocumentId → (3) agreement is sent for signature.

Upload a document to Adobe Sign as a transient document — the first step before creating an agreement for signature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adobe Acrobat Sign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all agreements waiting for signature"

**🤖 AI Agent:**
> You have **3 agreements** out for signature:

✍️ **Acme Corp NDA** — Sent to john@acme.com, viewed 1 hour ago ✅
✍️ **TechStart MSA** — Sent to legal@techstart.io, not yet viewed ⏳
✍️ **CloudBase SOW** — Signer 1 of 2 completed, waiting on CFO ✅

The TechStart MSA hasn't been opened — shall I send a reminder?


## ❓ FAQ

**Q: How do I get started with Adobe Sign?**
Subscribe, then enter your Adobe Sign access token (from **Adobe Admin Console → Acrobat Sign → API → Integration Key**). Your AI agent connects instantly to the global v6 API. No code, no complex setup — just connect and start signing.

**Q: Can my AI agent send a contract for signature to multiple people?**
Yes. Upload a document, then create an agreement with multiple signers in a specific order. Adobe Sign handles the sequential signing flow — Signer 1 gets notified first, then Signer 2 after completion, and so on. Your agent tracks each signer's progress in real time.

**Q: What if a signer hasn't signed yet — can I send a reminder?**
Just tell your agent "send a reminder for the Acme NDA." It sends an email reminder to all pending signers with an optional custom message. No tab-switching, no logging into Adobe Sign — your agent handles it directly from your conversation.

**Q: Can I access the legal audit trail for compliance?**
Yes. Every signed agreement has a tamper-proof audit trail showing exactly when it was created, viewed, signed, and by whom — with timestamps and IP addresses. Perfect for legal departments, regulated industries, and any business that needs proof of signing for compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adobe-acrobat-sign](https://vinkius.com/mcp/adobe-acrobat-sign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adobe Acrobat Sign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adobe-acrobat-sign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adobe Acrobat Sign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adobe-acrobat-sign": {
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
