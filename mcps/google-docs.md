# Google Docs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/google-docs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Read, write, and export Google Docs documents — a full text workflow for any AI agent through the official Docs API.

## Description
Connect your **Google Docs** documents to any AI agent through the official Google Docs API. Your agent can open a document, read it as structure or plain text, draft new docs, make targeted edits, and export to the format you actually need.

### What you can do

- **Read** — Fetch a document's full structure (sections, paragraphs, runs) or its flat plain text
- **Create** — Start a new document, optionally seeded with text
- **Edit** — Insert text at a character position or run find-and-replace with regex and capture groups
- **Export** — Download as PDF, DOCX, HTML, TXT, CSV, ePub, RTF or ODT (base64)

### How it works

1. Create a Google Cloud project, enable the Docs API, and create OAuth 2.0 client credentials (Web application)
2. Paste the Client ID and Client Secret into this server's credential fields
3. Connect your Google account through OAuth — the agent then acts only on documents that account can access

### Who is this for?

- **Writers & Researchers** — let an agent pull a doc's text, rewrite passages, and keep terminology consistent across a whole document
- **Automation** — turn notes into a formatted draft, apply bulk find-and-replace renames, and export the result without leaving the chat


## Available Tools (6)
- **get_document_text**: Use when the user wants to read or quote a doc, or when the agent needs the text to summarize or search it. Structure and formatting are dropped — use get_document when layout matters.

Read the plain text of a Google Doc
- **export_document**: Supported formats: application/pdf (default), application/vnd.openxmlformats-officedocument.wordprocessingml.document (.docx), text/html, text/csv, text/plain (.txt), application/epub+zip, application/rtf, and application/vnd.oasis.opendocument.text. Use when the user wants the doc as a file instead of reading it in place.

Export a Google Doc to another format
- **get_document**: Use when the agent needs to understand the layout before editing, or when the user asks for the content of a specific doc. The document ID is the long alphanumeric code in the Doc URL — not the URL itself. For a quick plain-text view instead of structure, use get_document_text.

Read the structure of a Google Doc
- **create_document**: Use when the user asks to start a fresh doc or to turn agent-generated text into a document. Provide a title and optionally the initial body text; an empty document is created when neither is given.

Create a new Google Doc
- **insert_text**: Use for adding content, comments, or notes. Character indices count from the start of the document text — locate an index with get_document_text and counting, since they shift after edits.

Insert text into a Google Doc
- **replace_text**: The match pattern may use standard regex with capture groups, and $1/$2 in the replacement refer to them. Use for find-and-replace: renaming a term, applying a style pass, or deleting (empty replacement). All occurrences are replaced in one operation.

Replace matching text in a Google Doc


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Docs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Turn these meeting notes into a formatted Google Doc."

**🤖 AI Agent:**
> Created 'Board sync — Sep 2026' and inserted the notes as sections: Decisions, Open items, Risks, and Next steps, with the action items listed under each. Want me to tighten the wording or reorder the sections?

---

**👤 You:**
> "Read my 'Investor update' doc and summarize it."

**🤖 AI Agent:**
> The doc covers the quarter in four parts: KPIs (MRR up 18% QoQ, churn steady), a product roadmap with two GA dates, the enterprise pipeline by stage, and an ask for board approval of the pricing change. Two risks are flagged in red in the risks section — those are the ones investors will poke at.

---

**👤 You:**
> "Replace every 'ACME Inc' in the doc with 'Acme Corp' and export it as PDF."

**🤖 AI Agent:**
> Replaced 6 occurrences of 'ACME Inc' with 'Acme Corp' in one pass, then exported the document as PDF (base64). The doc now reads consistently with the new name. Nothing else changed.


## ❓ FAQ

**Q: Which Google Cloud permissions are required?**
The OAuth flow requests only the Google Docs API scope. The agent can therefore read and modify documents that your connected Google account can access, and nothing beyond that scope.

**Q: How do replace_text regex and capture groups work?**
replace_text takes a regex pattern and a replacement string. Use $1, $2… in the replacement to insert captured groups. To rename a product across a whole doc, match the old name and replace with the new one in a single pass — every occurrence is updated.

**Q: What does export_document return?**
It returns the document converted to the requested format (pdf, docx, html, txt, csv, epub, rtf or odt) as a base64 string. Save the decoded bytes to a file to get a real downloadable document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/google-docs](https://vinkius.com/en/ai-agent-connect/google-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Docs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-docs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Docs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-docs": {
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
