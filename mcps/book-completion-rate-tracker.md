# Book Completion Rate Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/book-completion-rate-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and calculate reading progress and completion percentages for books.

## Description
This MCP server provides tools to monitor how much of a book a user has read. It allows for checking specific progress with `get_book_progress`, updating current page counts via `update_reading_progress`, viewing overall reading statistics with `get_user_reading_stats`, and filtering books by their global completion tiers using `list_books_by_completion_tier`.


## Available Tools (4)
- **get_book_progress**: Determines the current completion percentage for a specific user and book
- **get_user_reading_stats**: Aggregates completion data across all books for a single user
- **list_books_by_completion_tier**: Filters and retrieves books based on how much they have been read globally
- **update_reading_progress**: Updates the number of pages a user has read for a specific book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Book Completion Rate Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much of the book 'book_123' has user 'user_456' finished?"

**🤖 AI Agent:**
> User 'user_456' has completed 45% of 'book_123', having read 90 out of 200 pages.

---

**👤 You:**
> "Update my progress for 'book_789' to page 50."

**🤖 AI Agent:**
> Progress updated successfully. Your new completion rate for 'book_789' is 25%.

---

**👤 You:**
> "Show me books that have a global completion rate between 50% and 80%."

**🤖 AI Agent:**
> The following books have an average completion rate between 50% and 80%: 'book_abc' (62%), 'book_def' (75%).


## ❓ FAQ

**Q: How do I update my current page?**
You can use the `update_reading_progress` tool to set the current page number for a specific user and book.

**Q: Can I see my total reading statistics?**
Yes, the `get_user_reading_stats` tool provides an aggregate view of your average completion rate and books completed.

**Q: How is the completion rate calculated?**
The completion rate is the ratio of pages read to the total number of pages in the book, expressed as a percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/book-completion-rate-tracker](https://vinkius.com/en/ai-agent-connect/book-completion-rate-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Book Completion Rate Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `book-completion-rate-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Book Completion Rate Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "book-completion-rate-tracker": {
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
