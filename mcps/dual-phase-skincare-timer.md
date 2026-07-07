# Dual-Phase Skincare Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dual-phase-skincare-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates exact clock times for two-phase skincare steps.

## Description
Ensure precision in your chemical exfoliation or recovery routines. Using `generate_routine_timeline`, you can determine exactly when to apply and remove products based on your start time and phase durations. The tool also provides `calculate_total_routine_runtime` for total elapsed time and `validate_time_format` to ensure your timestamps are correct.


## Available Tools (3)
- **calculate_total_routine_runtime**: Calculates total routine runtime in minutes
- **generate_routine_timeline**: Generates a human-readable skincare routine timeline
- **validate_time_format**: g., "8:00 PM") and returns whether it is valid.

Validates if a time string is in a valid format


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dual-Phase Skincare Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I start my acid peel at 7:00 PM. Phase 1 is 10 mins, buffer is 5 mins, phase 2 is 15 mins. When do I finish?"

**🤖 AI Agent:**
> Apply Acid at 7:00 PM. Wash off at 7:10 PM. Apply Mask at 7:15 PM. Wash off at 7:30 PM.

---

**👤 You:**
> "What is the total time for a routine with 5 mins phase 1, 2 mins buffer, and 10 mins phase 2?"

**🤖 AI Agent:**
> The total runtime is 17 minutes.

---

**👤 You:**
> "Is '8:30 AM' a valid time format?"

**🤖 AI Agent:**
> Yes, the time format is valid.


## ❓ FAQ

**Q: How does it calculate the time?**
It adds the duration of phase one, the buffer period, and the duration of phase two to your starting time.

**Q: Can I use it for different products?**
Yes, any product with a defined application and removal window can be scheduled using `generate_routine_timeline`.

**Q: Does it support 24-hour format?**
Yes, the `validate_time_format` tool ensures your input is recognized in both 1s and 24-hour formats.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dual-phase-skincare-timer](https://vinkius.com/mcp/dual-phase-skincare-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dual-Phase Skincare Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dual-phase-skincare-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dual-Phase Skincare Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dual-phase-skincare-timer": {
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
