# Set-List Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/set-list-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your live performance with energy-driven song sequencing and musical transition analysis.

## Description
The Set-List Planner is a specialized tool for musicians to organize song sequences that optimize energy flow, musical compatibility, and performance stamina. Using the `optimize_set_sequence` tool, you can rearrange your tracks into an ideal energy arc--starting with a strong opening, moving through a mid-set valley, and reaching a powerful climax. You can also use `analyze_transition_smoothness` to evaluate how jarring key or tempo changes might be, and `extract_performance_metadata` to identify the best keys for vocal warm-ups and strategic break points during your set.


## Available Tools (3)
- **analyze_transition_smoothness**: Evaluates musical smoothness between songs
- **extract_performance_metadata**: Extracts preparation data from a set list
- **optimize_set_sequence**: Reorders songs into an optimized energy arc


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Set-List Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a list of 5 songs. Can you optimize the sequence for a standard energy arc?"

**🤖 AI Agent:**
> Please provide the JSON array of songs including their BPM, key, duration, and energy level so I can run `optimize_set_sequence` for you.

---

**👤 You:**
> "Are the transitions between these songs smooth: Song A (C Major, 120 BPM) and Song B (F# Major, 140 BPM)?"

**🤖 AI Agent:**
> No, that transition is likely to be 'Jarring' due to the large distance on the Circle of Fifths and the significant jump in tempo.

---

**👤 You:**
> "What is the most frequent key in my set list?"

**🤖 AI Agent:**
> The `extract_performance_metadata` tool identifies G Major as your primary warmup key, meaning most of your songs are in that key.


## ❓ FAQ

**Q: How does the energy curve optimization work?**
The `optimize_set_sequence` tool rearranges your songs to follow a 'Standard' pattern: a high-energy opening, a lower-energy middle section (the valley), and a high-energy finale (the climax).

**Q: Can I check if my song transitions are smooth?**
Yes, use the `analyze_transition_smoothness` tool. It calculates the distance between keys on the Circle of Fifths and measures tempo volatility to give you a smoothness rating.

**Q: How can I prepare for my vocal performance?**
Use `extract_performance_metadata` to find the `primaryWarmupKey`. This identifies the most frequent key in your set, helping you prepare your vocal range effectively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/set-list-planner](https://vinkius.com/mcp/set-list-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Set-List Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `set-list-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Set-List Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "set-list-planner": {
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
