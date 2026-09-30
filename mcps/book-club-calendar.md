# Book Club Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/book-club-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage reading cycles, meeting logistics, and discussion topics.

## Description
This MCP server connects AI agents to your book club's organizational data. It allows agents to retrieve scheduled reading cycles using `get_reading_cycles`, check meeting logistics like location and host via `get_meeting_details`, calculate book costs with `get_financial_summary`, and access curated conversation themes through `get_discussion_plan`.


## Available Tools (4)
- **get_reading_cycles**: Retrieves a list of all scheduled or past reading cycles
- **get_discussion_plan**: Retrieves the curated topics for a meeting
- **get_financial_summary**: Calculates the total book cost for a specific cycle
- **get_meeting_details**: Provides specific logistics for a scheduled meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Book Club Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the details for the next book club meeting?"

**🤖 AI Agent:**
> The next meeting for 'The Great Gatsby' is scheduled for June 15th at 7:00 PM at the Downtown Library, hosted by Sarah.

---

**👤 You:**
> "How much is the total cost for the current reading cycle?"

**🤖 AI Agent:**
> The total cost for the current cycle is $120.00, based on a book price of $15.00 per member.

---

**👤 You:**
> "What should we talk about during our next meeting?"

**🤖 AI Agent:**
> The primary theme is 'Social Class in the 1920s'. Discussion topics include the symbolism of the green light and the impact of wealth on character motivations.


## ❓ FAQ

**Q: How can I see upcoming book reading periods?**
You can use the `get_reading_cycles` tool and filter by the 'Planned' or 'In-Progress' status to see upcoming periods.

**Q: Where can I find the meeting location and host information?**
Use the `get_meeting_details` tool with the specific cycle ID to retrieve the date, time, location, and host name.

**Q: Can I find out how much the books will cost the group?**
Yes, the `get_financial_summary` tool provides the individual book cost and the total cost for all active members.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/book-club-calendar](https://vinkius.com/en/ai-agent-connect/book-club-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Book Club Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `book-club-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Book Club Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "book-club-calendar": {
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
