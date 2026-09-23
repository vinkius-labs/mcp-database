# Journal Entry Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/journal-entry-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze journal writing habits and entry counts.

## Description
This MCP server provides tools to track and analyze journal writing patterns. You can use `count_entries_in_range` to find total entries over a period, `get_entries_by_date` for specific daily counts, `get_user_frequency_tier` to determine engagement levels, and `get_entry_distribution` to see weekly activity patterns.


## Available Tools (4)
- **count_entries_in_range**: Calculates the total number of journal entries recorded between two specific dates
- **get_entries_by_date**: Retrieves the exact number of entries recorded on a specific calendar day
- **get_entry_distribution**: Provides a breakdown of entry counts grouped by day of the week to identify weekly patterns
- **get_user_frequency_tier**: Determines the engagement level of the user based on their writing habits over a defined period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Journal Entry Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many journal entries did I make between 2024-01-01 and 2024-01-31?"

**🤖 AI Agent:**
> You made 15 journal entries between 2024-01-01 and 2024-01-31, with an average of 0.48 entries per day.

---

**👤 You:**
> "How many entries did I write on 2024-05-20?"

**🤖 AI Agent:**
> You wrote 2 entries on 2024-05-20.

---

**👤 You:**
> "What is my writing engagement level for the last two weeks?"

**🤖 AI Agent:**
> Your engagement level is High Frequency, as you have been writing consistently over the last 14 days.


## ❓ FAQ

**Q: How can I see my total entries for the month?**
You can use the `count_entries_in_range` tool by providing the start and end dates for the month.

**Q: What is a frequency tier?**
A frequency tier is a categorization of your writing habits, such as High, Moderate, or Low, determined by `get_user_frequency_tier`.

**Q: Can I see which days I write most often?**
Yes, use `get_entry_distribution` to get a breakdown of entries by the day of the week.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/journal-entry-counter](https://vinkius.com/en/ai-agent-connect/journal-entry-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Journal Entry Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `journal-entry-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Journal Entry Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "journal-entry-counter": {
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
