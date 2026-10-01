# Manuscript Word Count Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/manuscript-word-count-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate daily writing targets and manage manuscript schedules.

## Description
This MCP server provides a specialized scheduling engine for authors. It calculates feasible daily writing targets by distributing remaining word counts over a specific timeframe. You can use `get_writing_schedule` to determine daily requirements, `validate_writing_window` to check schedule feasibility, `get_daily_breakdown` for a detailed calendar view, and `calculate_buffer_impact` to see how catch-up days reduce your daily workload.


## Available Tools (4)
- **calculate_buffer_impact**: Determine how much extra capacity is provided by adding catch-up days
- **get_daily_breakdown**: Generate a day-by-day list showing the type of each day in the schedule
- **get_writing_schedule**: Calculate the daily word count requirement and the number of active writing days available
- **validate_writing_window**: Ensure the requested timeframe and constraints are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Manuscript Word Count Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to write 50,000 words. I have written 5,000 so far. I start on 2024-01-01 and want to finish by 2024-03-01. How many words should I write daily?"

**🤖 AI Agent:**
> To reach your 50,000-word goal starting from 5,000 words, you need to write 45,000 more words. Over the 60 days between 2024-01-01 and 2024-03-01, your daily target is 750 words.

---

**👤 You:**
> "Show me a breakdown of my writing schedule from 2024-05-01 to 2024-05-10, excluding 2024-05-05."

**🤖 AI Agent:**
> Your schedule includes 9 writing days and 1 excluded day on 2024-05-05.

---

**👤 You:**
> "How much does adding 5 catch-up days reduce my daily target for a 10,000 word goal over 20 writing days?"

**🤖 AI Agent:**
> Adding 5 catch-up days reduces your daily target from 500 words to 400 words.


## ❓ FAQ

**Q: How do I calculate my daily word count goal?**
You can use the `get_writing_schedule` tool by providing your target words, current progress, start date, and deadline.

**Q: Can I exclude specific dates from my writing plan?**
Yes, you can provide a list of excluded dates to the tools to ensure they are not counted as active writing days.

**Q: What is the purpose of catch-up days?**
Catch-up days act as a buffer, allowing you to reduce your standard daily target or recover from missed goals using `calculate_buffer_impact`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/manuscript-word-count-plan](https://vinkius.com/en/ai-agent-connect/manuscript-word-count-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Manuscript Word Count Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `manuscript-word-count-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Manuscript Word Count Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "manuscript-word-count-plan": {
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
