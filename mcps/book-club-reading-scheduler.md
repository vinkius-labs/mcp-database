# Book Club Reading Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/book-club-reading-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate optimized reading schedules that respect chapter integrity and availability.

## Description
This MCP server provides a complete toolkit for book clubs to manage their reading progress. Use `generate_reading_schedule` to create a primary plan that respects chapter boundaries and your available reading days. If you prefer a more consistent daily workload, `get_balanced_schedule` will redistribute the page load to minimize daily variance. You can also use `validate_reading_constraints` to check if your goals are mathematically possible, or `get_chapter_summary` to analyze the book's structure. It is designed to handle blackout dates and maximum daily page limits to ensure a realistic reading experience.


## Available Tools (4)
- **generate_reading_schedule**: Creates a primary reading schedule based on book structure and user constraints
- **get_balanced_schedule**: Provides an alternative schedule that minimizes the variance in daily page counts
- **get_chapter_summary**: Provides metadata about the book's structure to help the user decide on reading increments
- **validate_reading_constraints**: Checks if a user's specific constraints are mathematically capable of completing the book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Book Club Reading Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a reading schedule for a 300-page book with 10 chapters (each 30 pages). I can read on 2024-05-01, 2024-05-03, and 2024-05-05. My meeting is on 2024-05-06. I can read 40 pages per day."

**🤖 AI Agent:**
> Your reading schedule is set: May 1st (Chapters 1-2, 60 pages), May 3rd (Chapters 3-5, 90 pages - Note: this exceeds 40 pages, please adjust), May 5th (Chapters 6-10, 150 pages). Wait, let me recalculate based on your 40 page limit: May 1st (30 pages), May 3rd (30 pages), May 5th (30 pages)... [Simulated response based on constraints]

---

**👤 You:**
> "Is it possible to finish a 500-page book by 2024-06-01 if I only have 5 reading days and can read 50 pages per day?"

**🤖 AI Agent:**
> No, it is not possible. With 5 reading days and a limit of 50 pages per day, your maximum capacity is 250 pages, which is less than the 500 pages required.

---

**👤 You:**
> "Give me a summary of a book with chapters at pages 1-20, 21-50, and 51-100."

**🤖 AI Agent:**
> The book has 3 chapters. The average chapter length is 30 pages. The longest chapter is 30 pages and the shortest chapter is 20 pages.


## ❓ FAQ

**Q: Can I split chapters between different days?**
By default, the tool respects chapter integrity. However, you can set the `allowChapterSplitting` parameter to true if you want to break chapters into multiple days.

**Q: How do I handle days when I cannot read?**
You can provide a list of `blackoutDates` to the `generate_reading_schedule` tool to ensure no reading is assigned to those specific days.

**Q: What happens if my reading goal is impossible?**
If the total pages exceed your capacity based on `maxPagesPerDay` and available dates, the `isLate` flag will be true. You can use `validate_reading_constraints` to check feasibility before generating a full schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/book-club-reading-scheduler](https://vinkius.com/en/ai-agent-connect/book-club-reading-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Book Club Reading Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `book-club-reading-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Book Club Reading Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "book-club-reading-scheduler": {
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
