# Crochet Gauge Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/crochet-gauge-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Recalculate stitch and row counts based on your crochet gauge.

## Description
This MCP server provides precision tools for crochet enthusiasts to adjust pattern instructions when their personal tension differs from the designer's. Use `convert_stitch_count` to find the new stitch count for a specific width, `convert_row_count` to adjust height, `calculate_size_deviation` to predict size errors, and `get_gauge_comparison` to determine if your tension is tighter or looser than the pattern.


## Available Tools (4)
- **calculate_size_deviation**: Determines how much the physical dimensions of a project will change if the user follows the pattern without adjusting
- **convert_row_count**: Calculates the required number of rows to achieve the target height based on gauge differences
- **convert_stitch_count**: Calculates the required number of stitches to achieve the target dimension based on gauge differences
- **get_gauge_comparison**: Provides a qualitative assessment of the user's tension relative to the pattern


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crochet Gauge Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My pattern says 20 stitches for 4 inches, but I got 22 stitches for 4 inches. How many stitches should I work for a 40 inch wide blanket?"

**🤖 AI Agent:**
> You should work 36 stitches to achieve a 40 inch width with your gauge.

---

**👤 You:**
> "Is my tension tighter or looser than the pattern? The pattern is 15 rows per 4 inches and I am getting 12 rows per 4 inches."

**🤖 AI Agent:**
> Your tension is looser than the pattern.

---

**👤 You:**
> "If I follow a pattern with 10 stitches per 4 inches but my gauge is 12 stitches per 4 inches, how much will my 10 inch square deviate?"

**🤖 AI Agent:**
> Your finished square will be approximately 8.33 inches wide, resulting in a 16.67% size deviation.


## ❓ FAQ

**Q: How do I use this to fix a pattern that is too small?**
If your project is too small, your gauge is likely tighter than the pattern. Use `convert_stitch_count` with your user gauge to calculate the higher number of stitches needed to reach the target width.

**Q: What is gauge in crochet?**
Gauge is the number of stitches and rows that fit into a specific unit of measurement, such as 4 inches. It determines the density of your crochet fabric.

**Q: Can I use this for knitting too?**
While designed for crochet, the mathematical principles of gauge adjustment apply to knitting as well.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/crochet-gauge-converter](https://vinkius.com/en/ai-agent-connect/crochet-gauge-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crochet Gauge Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crochet-gauge-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crochet Gauge Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crochet-gauge-converter": {
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
