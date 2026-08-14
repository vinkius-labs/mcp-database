# Knitting Gauge Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knitting-gauge-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert garment dimensions and shaping rules into precise stitch counts and schedules.

## Description
This MCP server provides technical precision for knitters and crocheters. It converts target garment dimensions and specific shaping instructions into exact stitch counts, row counts, and chronological shaping schedules. Use `calculate_base_dimensions` to find your starting cast-on count and total rows based on your gauge. Use `generate_shaping_schedule` to create a row-by-row roadmap for increases and decreases. Finally, use `estimate_yarn_consumption` to predict the total length of yarn required for your project based on the weight class of your yarn.


## Available Tools (3)
- **calculate_base_dimensions**: Determines the fundamental stitch and row counts required to meet the target physical dimensions
- **estimate_yarn_consumption**: Predicts the total length of yarn needed to complete the project
- **generate_shaping_schedule**: Creates a precise chronological roadmap of every row where the stitch count changes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knitting Gauge Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to knit a piece that is 40cm wide and 60cm high. My stitch gauge is 20 sts per 10cm and my row gauge is 28 rows per 10cm. How many stitches should I cast on?"

**🤖 AI Agent:**
> You should cast on 80 stitches.

---

**👤 You:**
> "I have 80 stitches. I need to decrease 1 stitch each side every 4th row 5 times. What is my shaping schedule?"

**🤖 AI Agent:**
> The shaping schedule is: Row 4: decrease 1 st each side (78 sts), Row 8: decrease 1 st each side (76 sts), Row 12: decrease 1 st each side (74 sts), Row 16: decrease 1 st each side (72 sts), Row 20: decrease 1 st each side (70 sts).

---

**👤 You:**
> "I worked 5000 stitches using Worsted weight yarn. How much yarn do I need?"

**🤖 AI Agent:**
> You will need approximately 450 meters of yarn.


## ❓ FAQ

**Q: How do I calculate my starting stitches?**
You can use the `calculate_base_dimensions` tool. Provide your target width in cm, target height in cm, and your stitch and row gauge to get the exact cast-on count.

**Q: Can I use this for crochet patterns?**
Yes, the logic for stitch and row counts applies to both knitting and crochet projects.

**Q: How does the yarn estimation work?**
The `estimate_yarn_consumption` tool uses the total number of stitches worked and a multiplier specific to your yarn weight class (like Worsted or Bulky) to predict the required length.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knitting-gauge-calculator](https://vinkius.com/mcp/knitting-gauge-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knitting Gauge Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knitting-gauge-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knitting Gauge Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knitting-gauge-calculator": {
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
