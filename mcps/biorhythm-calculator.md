# Biorhythm Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/biorhythm-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and analyze the three primary biological cycles--physical, emotional, and intellectual.

## Description
This MCP server provides tools to quantify your biological rhythms. Use `get_rhythm_status` to determine the current energy percentages for physical, emotional, and intellectual cycles on any given date. You can also use `check_critical_windows` to identify upcoming dates of biological instability where cycles cross zero, or `locate_rhythm_peaks` to find when each cycle will reach its maximum positive amplitude.


## Available Tools (3)
- **check_critical_windows**: Identify upcoming dates where biological instability is expected due to cycle transitions
- **locate_rhythm_peaks**: Find the next occurrence of maximum biological strength for each cycle
- **get_rhythm_status**: Determine the current biological standing and energy percentages for all three cycles on a specific date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Biorhythm Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current biorhythm status for today?"

**🤖 AI Agent:**
> The `get_rhythm_status` tool would return the current percentages and amplitudes for your physical, emotional, and intellectual cycles based on today's date.

---

**👤 You:**
> "Are there any critical days coming up next week?"

**🤖 AI Agent:**
> By using `check_critical_windows` with a start and end date for next week, the tool will list any dates where your biological cycles are crossing zero.

---

**👤 You:**
> "When is my next intellectual peak?"

**🤖 AI Agent:**
> The `locate_rhythm_peaks` tool can be used to find the exact date when your intellectual cycle reaches its maximum positive amplitude.


## ❓ FAQ

**Q: What are the three biorhythm cycles?**
The three primary cycles are Physical (23 days), Emotional (28 days), and Intellectual (33 days).

**Q: What is a critical day?**
A critical day occurs when any of the three biological cycles cross the zero-point, indicating a period of transition and potential instability.

**Q: How can I find my next peak performance day?**
You can use the `locate_rhythm_peaks` tool to identify upcoming dates when each cycle reaches its maximum positive amplitude.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/biorhythm-calculator](https://vinkius.com/mcp/biorhythm-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Biorhythm Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `biorhythm-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Biorhythm Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "biorhythm-calculator": {
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
