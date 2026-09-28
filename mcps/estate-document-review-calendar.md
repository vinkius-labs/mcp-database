# Estate Document Review Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/estate-document-review-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and schedule critical estate document reviews based on life events and professional requirements.

## Description
This MCP server provides a structured system for managing the lifecycle of estate documents. It helps users track when documents like Wills or Trusts need review due to time intervals or specific life changes. Use `get_review_calendar` to identify upcoming review dates, `generate_appointment_checklist` to prepare for professional meetings, `get_document_access_map` to locate documents and authorized contacts, and `record_document_update` to maintain a historical log of all changes. It connects your AI assistant to your estate management workflow via Vinkius Edge.


## Available Tools (4)
- **generate_appointment_checklist**: Generates a checklist for a professional document review meeting
- **get_document_access_map**: Maps documents to their storage locations and authorized contacts
- **get_review_calendar**: Returns a list of upcoming review events based on intervals or life changes
- **record_document_update**: Records a historical log of a document update


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Estate Document Review Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When should I next review my estate documents?"

**🤖 AI Agent:**
> Your next review for the 'Last Will and Testament' is scheduled for October 15, 2025, due to your 3-year periodic review interval.

---

**👤 You:**
> "Help me prepare for my meeting to review my Will and Trust."

**🤖 AI Agent:**
> Here is your checklist: 1. Verify current beneficiaries (High Priority), 2. Confirm executor contact details (Medium Priority), 3. Review storage locations for physical copies (Low Priority). Professional verification is required for these documents.

---

**👤 You:**
> "Where is my Power of Attorney stored and who can access it?"

**🤖 AI Agent:**
> The Power of Attorney is stored in your Secure Digital Vault, and access is authorized for John Doe and Jane Smith.


## ❓ FAQ

**Q: How do I know when my documents need updating?**
You can use the `get_review_calendar` tool to see upcoming review dates triggered by your defined intervals or specific life events.

**Q: Can I prepare for a meeting with my lawyer using this tool?**
Yes, the `generate_appointment_checklist` tool creates a structured list of tasks and goals to help you prepare for professional reviews.

**Q: Where can I find my document locations?**
The `get_document_access_map` tool provides a mapping of your documents to their storage locations and the authorized contacts who can access them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/estate-document-review-calendar](https://vinkius.com/en/ai-agent-connect/estate-document-review-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Estate Document Review Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `estate-document-review-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Estate Document Review Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "estate-document-review-calendar": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
