# Recording Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recording-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate precise studio schedules, cost estimates, and completion risk assessments for music production.

## Description
The Recording Session Planner is a specialized tool designed to organize instrument tracking in a sequential layering workflow. It calculates detailed timelines using the `get_instrument_timeline` tool, ensuring that drums, bass, guitar, and vocals are scheduled with appropriate buffers for setup and tuning. Beyond scheduling, you can use `calculate_session_cost` to project total studio expenditures based on your session duration and hourly rates. Additionally, the `check_completion_probability` tool provides a critical risk assessment by comparing your estimated recording time against your booked studio window, helping you identify potential delays before they happen.


## Available Tools (3)
- **calculate_session_cost**: Estimates the total financial expenditure for the session
- **check_completion_probability**: Assesses the likelihood of completing the session on time
- **get_instrument_timeline**: Calculates the recording timeline for each instrument


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recording Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 3 songs to record. I expect about 2 takes per instrument, and each song is roughly 4 minutes long. I want a 10-minute buffer for setup between parts. What will my timeline look like?"

**🤖 AI Agent:**
> Your recording sequence starts with Drums, followed by Bass, Guitar, and Vocals. Each part includes your 10-minute buffer, ensuring a structured session.

---

**👤 You:**
> "If my session is expected to last 5 hours and the studio rate is $100 per hour, what is my estimated cost?"

**🤖 AI Agent:**
> $500.00 is the estimated total cost for your 5-hour session.

---

**👤 You:**
> "I have booked 4 hours of studio time, but my calculated recording duration is 4.5 hours. What is the probability I will finish on time?"

**🤖 AI Agent:**
> The completion probability is 0% with a High risk level, as your required duration exceeds your available studio window.


## ❓ FAQ

**Q: How does the instrument timeline calculation work?**
The tool follows a fixed hierarchy: Drums → Bass → Guitar → Vocals. It uses `get_instrument_timeline` to calculate the start and end times for each part, including buffers for setup and tuning.

**Q: Can I estimate my total studio costs?**
Yes, by using the `calculate_session_cost` tool, you can provide your expected session hours and hourly rate to get a projected total cost.

**Q: How is the risk of running over time assessed?**
The `check_completion_probability` tool compares your calculated recording duration against your available studio hours to determine a completion percentage and risk level (Low, Medium, or High).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recording-session-planner](https://vinkius.com/mcp/recording-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recording Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recording-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recording Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recording-session-planner": {
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
