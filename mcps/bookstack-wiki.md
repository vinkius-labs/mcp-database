# BookStack (Wiki) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bookstack-wiki)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage your BookStack wiki directly from your AI agent — search, read, create, and organize pages, chapters, and books with ease.

## Description
Connect your **BookStack** instance to any AI agent and turn your documentation into an interactive knowledge base through natural conversation.

### What you can do

- **Content Hierarchy** — List and manage shelves, books, chapters, and pages using `list_shelves`, `list_books`, and `list_pages` to maintain perfect organization.
- **Smart Search** — Find exactly what you need across your entire wiki instance with the powerful `search` tool.
- **Full Content Lifecycle** — Create, update, or delete pages and chapters directly from your agent to keep documentation fresh.
- **Multi-format Export** — Use `export_page` to retrieve content in PDF, Markdown, HTML, or Plaintext formats for external use.
- **System Oversight** — Monitor your instance with `get_system_status`, check `list_audit_log` for recent changes, or manage the `list_recycle_bin`.
- **Attachments** — Manage file attachments linked to your documentation using the dedicated attachment tools.

### How it works

1. Subscribe to this server
2. Enter your BookStack URL, Token ID, and Token Secret
3. Start managing your knowledge base from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Documentation Leads** — maintain and organize large wikis without manual navigation
- **Engineering Teams** — search for technical specs and update READMEs directly from the IDE
- **Support Teams** — quickly find and export help articles for customers


## Available Tools (32)
- **create_page**: Requires either book_id or chapter_id, name, and html or markdown.

Create a new page in BookStack
- **create_shelf**: Create a new shelf
- **delete_attachment**: Delete an attachment
- **delete_book**: Delete a book
- **delete_chapter**: Delete a chapter
- **delete_page**: Delete a page (moves to recycle bin)
- **delete_shelf**: Delete a shelf
- **export_book**: Export book content
- **export_chapter**: Export chapter content
- **export_page**: Export page content
- **get_attachment**: Get details for a specific attachment
- **get_book**: Get details for a specific book
- **get_chapter**: Get details for a specific chapter
- **get_page**: Get details for a specific page
- **get_shelf**: Get details for a specific shelf
- **get_system_status**: Check system version and status
- **list_attachments**: List all attachments in BookStack
- **list_audit_log**: View system activity audit log
- **list_books**: List all books in BookStack
- **list_chapters**: List all chapters in BookStack
- **list_pages**: Supports pagination, sorting, and filtering.

List all pages in BookStack
- **list_recycle_bin**: List deleted items in the recycle bin
- **list_shelves**: List all shelves in BookStack
- **search**: Search across all content in BookStack
- **update_attachment**: Update an existing attachment
- **update_book**: Update an existing book
- **update_chapter**: Update an existing chapter
- **update_page**: Update an existing page
- **update_shelf**: Update an existing shelf
- **create_attachment**: Create a new attachment link
- **create_book**: Create a new book
- **create_chapter**: Create a new chapter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BookStack (Wiki)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my BookStack wiki for 'security policy'."

**🤖 AI Agent:**
> I found 3 results for 'security policy'. The most relevant is a page titled 'Internal Security Guidelines' (ID: 42) in the 'Compliance' book. Would you like me to read its content?

---

**👤 You:**
> "Create a new page titled 'Onboarding' in book ID 5 with some basic HTML content."

**🤖 AI Agent:**
> I've created the 'Onboarding' page in Book ID 5. The new Page ID is 128. You can now view or update it using that ID.

---

**👤 You:**
> "Export the 'API Reference' page (ID: 88) as a PDF."

**🤖 AI Agent:**
> I have triggered the export for page ID 88 in PDF format. The content is being processed for download.


## ❓ FAQ

**Q: Can I search across all my books and chapters at once?**
Yes! Use the `search` tool with your query string. It will return relevant results from pages, chapters, and books across your entire BookStack instance.

**Q: Is it possible to retrieve a page's content in Markdown format?**
Absolutely. Use the `export_page` tool and set the format to 'markdown'. You can also export to PDF, HTML, or plaintext.

**Q: How do I see what was recently deleted?**
You can use the `list_recycle_bin` tool to view items that have been moved to the recycle bin before they are permanently removed from the system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bookstack-wiki](https://vinkius.com/mcp/bookstack-wiki)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BookStack (Wiki)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bookstack-wiki` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BookStack (Wiki)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bookstack-wiki": {
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
