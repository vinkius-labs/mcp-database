# Deterministic Datetime Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-datetime-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI with exact temporal math. Deterministically calculate date differences, leap years, and add business days (skipping weekends) 100% locally.

## Description
Language Models are infamously bad at calendar math. If you ask an AI to "Add 45 business days to October 12th", it will almost always guess wrong because it cannot programmatically skip weekends and account for varying month lengths. The Datetime Operations MCP solves this by offloading temporal calculations to a strict V8 Javascript engine.

### The Superpowers
- **Business Day Math:** Add or subtract days while perfectly skipping Saturdays and Sundays. Essential for SLA calculations, billing cycles, or delivery estimates.
- **Exact Date Differences:** Need to know exactly how many days, months, or years passed between two dates? Stop guessing and get mathematically perfect totals instantly.
- **Leap Year Logic:** Flawlessly implements the Gregorian leap year algorithm (`% 4 == 0 && % 100 !== 0`).
- **Privacy First (Local):** Executes completely locally. Zero API latency.


## Available Tools
- **add_business_days**: Adds or subtracts a specific number of business days (skipping weekends) from a given date
- **calculate_date_difference**: Calculates the exact mathematical difference between two dates in days, months, and years
- **check_leap_year**: Checks if a specific year is a leap year using the exact Gregorian calendar algorithm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Datetime Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the deadline: Add 15 business days to 2024-10-01."

**🤖 AI Agent:**
> Using the add_business_days tool: The final date is 2024-10-22.

---

**👤 You:**
> "Exactly how many days passed between 2020-01-01 and today?"

**🤖 AI Agent:**
> Using the calculate_date_difference tool: Exactly 1568 days (or 4 years and 3 months) have passed.


## ❓ FAQ

**Q: Why use an MCP for adding days to a date?**
AI models predict tokens, they don't "compute" calendars. When crossing months (e.g., February 28th to March 1st) or calculating Business Days, LLMs hallucinate dates frequently. This MCP forces exact algorithmic execution.

**Q: Are public holidays supported?**
Currently, `add_business_days` only skips weekends (Saturdays and Sundays). True holiday calculation requires country-specific data which violates the zero-dependency nature of this core utility.

**Q: Is this tool secure and local?**
Yes. It executes 100% locally using standard Date parsing built into V8. No cloud dependencies or API calls are used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-datetime-engine](https://vinkius.com/mcp/deterministic-datetime-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Datetime Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deterministic-datetime-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Datetime Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-datetime-engine": {
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
