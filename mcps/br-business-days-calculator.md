# BR Business Days Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/br-business-days-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop LLMs from calculating SLAs incorrectly. An local, deterministic engine that adds business days while perfectly avoiding weekends and Brazilian national holidays.

## Description
LLMs cannot reliably calculate SLAs or business delivery times. If you ask an AI to 'add 5 business days to Feb 10th', it will frequently ignore Carnival or count a Saturday. This MCP solves this by providing a static, local-first calculation engine that perfectly handles Brazilian national holidays and weekends.

### The Superpowers

- **Flawless SLA Math:** Guarantee that your agents' promised delivery dates are exactly right, automatically skipping weekends and static/dynamic BR holidays.
- **Zero Latency & 100% Local:** Unlike our global `business-timezone-scheduler` that uses the Nager.Date API, this engine uses a hardcoded Brazilian holiday list in the V8 isolate. Zero external network calls. Instant execution.
- **Absolute Determinism:** Eliminates the hallucination of non-existent business days, bringing enterprise reliability to AI agents.


## Available Tools (2)
- **add_business_days**: Pass a starting date and the number of days to add (use negative values to subtract). The engine skips weekends and Brazilian holidays automatically.

Adds or subtracts X Brazilian business days from a given date
- **is_business_day**: Pass the date as an ISO string (YYYY-MM-DD). The engine accounts for all Brazilian national holidays and weekends.

Checks if a given date is a Brazilian business day (excludes weekends and BR national holidays)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BR Business Days Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a 10-business-day delivery SLA starting from `2024-02-09` (Brazil)."

**🤖 AI Agent:**
> ✅ **Business SLA Date:** `2024-02-27` (Skipped Carnival holidays and weekends).

---

**👤 You:**
> "Is `2024-11-15` counted as a valid business day for banking operations in Brazil?"

**🤖 AI Agent:**
> ✅ **Validation:** False. `2024-11-15` is a static Brazilian National Holiday (Republic Proclamation).

---

**👤 You:**
> "Add exactly 1 business day to `2024-03-28` (Thursday before Easter)."

**🤖 AI Agent:**
> ✅ **New Date:** `2024-04-01` (Skipped Good Friday `03-29` and the weekend).


## ❓ FAQ

**Q: Does it require an external API?**
No! It uses a statically compiled list of Brazilian national holidays.

**Q: Does it skip weekends automatically?**
Yes, Saturdays and Sundays are ignored.

**Q: Are Carnival and Easter supported?**
Yes, the dynamic dates for these holidays are embedded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/br-business-days-calculator](https://vinkius.com/mcp/br-business-days-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BR Business Days Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `br-business-days-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BR Business Days Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "br-business-days-calculator": {
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
