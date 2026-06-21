# Salesforce Files & Notes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-files-notes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search files, manage attachments, create notes, and access documents linked to any Salesforce record through natural conversation.

## Description
Connect **Salesforce Files & Notes** to any AI agent.

### What you can do
- **Files** — Search and list recent files with type, size, and owner
- **Versions** — View version history of any document
- **Attachments** — Get legacy attachments on any record
- **Linked Files** — Find all documents linked to a specific record
- **Notes** — Search and create notes attached to records

### Who is this for?
- **Sales Teams** — Find proposals and contracts instantly
- **Support** — Access case attachments without tab-switching
- **Operations** — Track document versions and ownership


## Available Tools
- **sf_create_note**: Create a new Note attached to a record
- **sf_get_attachments**: Get attachments on a specific record
- **sf_file_details**: Get all versions of a specific file (ContentDocument)
- **sf_linked_files**: Get files linked to a specific record
- **sf_recent_files**: List the most recently modified files in Salesforce
- **sf_search_files**: Returns file type, size, owner, and modification date.

Search files (ContentVersion) in Salesforce by title
- **sf_search_notes**: Returns title, body preview, creator, and dates.

Search Notes in Salesforce by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Files & Notes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all files related to the Acme account"

**🤖 AI Agent:**
> 📎 **Files linked to Acme Corp**
| Name | Type | Size | Date |
|---|---|---|---|
| Proposal_Q1.pdf | PDF | 2.3MB | Mar 15 |
| Contract_v2.docx | WORD | 450KB | Mar 22 |
| NDA_signed.pdf | PDF | 1.1MB | Jan 10 |

---

**👤 You:**
> "Search for files named proposal"

**🤖 AI Agent:**
> 📂 Found 5 files matching "proposal":
1. Proposal_Q1_2024.pdf (2.3MB)
2. Sales_Proposal_Template.docx (800KB)
3. Proposal_v3_final.pdf (1.5MB)

---

**👤 You:**
> "Create a note on the Acme account: Follow up next week about renewal"

**🤖 AI Agent:**
> 📝 **Note Created!**
- Title: Follow up next week about renewal
- Parent: Acme Corp
- Created: Just now


## ❓ FAQ

**Q: What file types are supported?**
All files stored in Salesforce CRM: PDFs, images, documents, spreadsheets — any ContentDocument or Attachment.

**Q: Can I create notes?**
Yes! Create Notes attached to any parent record (Account, Contact, Case, Opportunity).

**Q: Can I see file versions?**
Yes — view all versions of a ContentDocument with size, uploader, and modification date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-files-notes](https://vinkius.com/mcp/salesforce-files-notes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Files & Notes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salesforce-files-notes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Files & Notes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-files-notes": {
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
