# Reading Plan Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reading-plan-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divide books or chapters into daily reading targets leading up to specific deadlines.

## Description
Reading Plan Builder helps you manage your reading goals by breaking down large volumes of content into manageable daily tasks. Use `get_reading_velocity` to estimate how long a book will take, `calculate_plan_distribution` to create a custom schedule with linear or front-loaded pacing, and `validate_reading_capacity` to ensure your plan stays within your historical reading habits. You can also use `summarize_plan_metrics` to get a quick overview of your progress and targets.


## Available Tools (4)
- **calculate_plan_distribution**: Calculates the specific daily targets for a book given a deadline and a preferred pacing style
- **get_reading_velocity**: Determines the estimated time required to complete a book based on the user's reading speed
- **summarize_plan_metrics**: Provides a high-level overview of a generated plan for quick review
- **validate_reading_capacity**: Checks if a proposed reading plan is too intense for the user's historical reading patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reading Plan Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 300-page book and I read 10 pages a day. How many days will it take me to finish?"

**🤖 AI Agent:**
> It will take you 30 days to finish the book.

---

**👤 You:**
> "Create a reading plan for a 500-page book starting today (2024-01-01) and ending on 2024-01-20 using linear pacing."

**🤖 AI Agent:**
> Your daily target is 25 pages per day from 2024-01-01 to 2024-01-20.

---

**👤 You:**
> "I usually read 5 pages a day. Is a plan to read 20 pages a day too much?"

**🤖 AI Agent:**
> Yes, that plan has an intensity score of 4.0, which is significantly higher than the recommended limit.


## ❓ FAQ

**Q: How do I estimate how long it will take to finish my book?**
You can use the `get_reading_velocity` tool. Provide the total number of pages, chapters, or words, and your daily reading speed to get an estimated number of days.

**Q: Can I choose different pacing styles for my reading plan?**
Yes, when using `calculate_plan_distribution`, you can choose between 'linear' pacing for equal daily amounts or 'front-loaded' pacing to do more reading at the beginning.

**Q: How can I check if my reading plan is too difficult?**
Use the `validate_reading_capacity` tool. By comparing your proposed daily target against your historical average, the tool provides an intensity score to show if the plan is reasonable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reading-plan-builder](https://vinkius.com/en/ai-agent-connect/reading-plan-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reading Plan Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reading-plan-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reading Plan Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reading-plan-builder": {
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
