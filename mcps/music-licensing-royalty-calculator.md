# Music Licensing Royalty Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/music-licensing-royalty-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate royalties for sync, mechanical, performance, and print music licensing.

## Description
This MCP server provides a precise engine for estimating musical royalty payouts across various usage types. Use `calculate_sync_royalty` to estimate fees for visual media, `calculate_mechanical_royalty` for physical or digital reproductions, `calculate_performance_royalty` for public broadcasts and live events, and `calculate_print_royalty` for sheet music sales. The tool calculates the total royalty amount and provides a breakdown between the composer's share and the publisher's share based on industry standards like ASCAP, BMI, SESAC, and the Copyright Royalty Board.


## Available Tools (4)
- **calculate_mechanical_royalty**: Estimate royalties generated from the reproduction of music copies
- **calculate_performance_royalty**: Estimate royalties for public broadcasts or live performances
- **calculate_print_royalty**: Estimate royalties for the sale of sheet music and lyrics
- **calculate_sync_royalty**: Estimate the fee for synchronizing music with visual media


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Music Licensing Royalty Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much royalty will I earn from 10,000 digital copies of a 3-minute song in the USA?"

**🤖 AI Agent:**
> $910.00 total royalty ($455.00 for the composer and $455.00 for the publisher).

---

**👤 You:**
> "Estimate the sync fee for a 30-second advertisement in Europe."

**🤖 AI Agent:**
> $150.00 total royalty ($75.00 for the composer and $75.00 for the publisher).

---

**👤 You:**
> "What is the estimated performance royalty for a live concert with 5,000 people in the USA?"

**🤖 AI Agent:**
> $250.00 total royalty ($125.00 for the composer and $125.00 for the publisher).


## ❓ FAQ

**Q: How does the mechanical royalty calculation work?**
For tracks five minutes or less, a fixed rate of $0.091 per copy is applied. For longer tracks, a different tier applies, and all totals are adjusted by the selected territory multiplier.

**Q: Does the tool account for the split between composer and publisher?**
Yes, every calculation returns a breakdown showing exactly how much of the total royalty belongs to the composer and how much belongs to the publisher.

**Q: Which territories are supported?**
The tool supports calculations for the USA and Europe, applying specific multipliers to reflect different legal frameworks and market scales.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/music-licensing-royalty-calculator](https://vinkius.com/mcp/music-licensing-royalty-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Music Licensing Royalty Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `music-licensing-royalty-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Music Licensing Royalty Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "music-licensing-royalty-calculator": {
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
