# Library Book Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/library-book-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Manage book lifecycles, reading progress, and return logistics.

## Description
This MCP server provides tools to manage the complete lifecycle of library books. Use `get_book_status` to check loan details and reading progress, `calculate_reading_forecast` to predict if a user will finish on time, `manage_hold_request` to handle book reservations, and `get_return_logistics` to organize book returns into transport groups.


## Available Tools (4)
- **calculate_reading_forecast**: Predicts whether a user will finish a book before it is due based on their current speed
- **get_book_status**: Provides a comprehensive overview of a specific book's current lifecycle state
- **get_return_logistics**: Organizes books that need to be returned into logical groups for transport
- **manage_hold_request**: Handles the reservation of a book when it is unavailable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Library Book Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of book ID 'BK-9921'?"

**🤖 AI Agent:**
> Book BK-9921 is currently on loan. It has 5 days remaining until the due date, and the user has completed 45% of the book.

---

**👤 You:**
> "Will the user finish book 'BK-4432' before it is due?"

**🤖 AI Agent:**
> Yes, based on the current reading pace, the user is expected to finish the book on October 12th, which is before the due date.

---

**👤 You:**
> "Group the returns for trip 'TRIP-001'."

**🤖 AI Agent:**
> The returns for TRIP-001 have been organized into 2 groups with a total weight of 12.5kg.


## ❓ FAQ

**Q: How can I check if a book is overdue?**
You can use the `get_book_status` tool to retrieve the current status and penalty details for any book.

**Q: Can I predict when a user will finish a book?**
Yes, the `calculate_reading_forecast` tool uses current reading pace to estimate the finish date.

**Q: How do I manage book reservations?**
Use the `manage_hold_request` tool to place or cancel a hold for a specific book.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/library-book-plan](https://vinkius.com/en/ai-agent-connect/library-book-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Library Book Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `library-book-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Library Book Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "library-book-plan": {
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
