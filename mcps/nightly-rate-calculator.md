# Nightly Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nightly-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate average nightly rates from total room costs and stay duration.

## Description
This MCP server provides tools to calculate nightly rates for hospitality bookings. Use `get_nightly_rate` to find the average cost per night, `validate_stay_duration` to ensure stay lengths are valid, `get_stay_summary` for a full financial breakdown, or `bulk_calculate_rates` to process multiple bookings at once.


## Available Tools (4)
- **bulk_calculate_rates**: 
- **get_stay_summary**: 
- **get_nightly_rate**: 
- **validate_stay_duration**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nightly Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the nightly rate for a stay costing $500 for 5 nights?"

**🤖 AI Agent:**
> The nightly rate is $100.

---

**👤 You:**
> "Give me a summary for a $1200 booking over 4 nights."

**🤖 AI Agent:**
> Total amount: $1200, Nights: 4, Average rate: $300.

---

**👤 You:**
> "Is a stay of 0 nights valid?"

**🤖 AI Agent:**
> No, a stay of 0 nights is not a valid duration.


## ❓ FAQ

**Q: How do I calculate the rate for a single booking?**
You can use the `get_nightly_rate` tool by providing the total room cost and the number of nights stayed.

**Q: Can I process multiple bookings at the same time?**
Yes, the `bulk_calculate_rates` tool allows you to process a list of booking objects in a single request.

**Q: What happens if I provide zero nights?**
The tools will return an error, as a valid stay must consist of at least one night.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nightly-rate-calculator](https://vinkius.com/en/ai-agent-connect/nightly-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nightly Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nightly-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nightly Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nightly-rate-calculator": {
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
