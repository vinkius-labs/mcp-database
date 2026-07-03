# Yarn Length Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yarn-length-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Estimate yarn length for knitting and crochet projects.

## Description
A precision estimator for knitters and crocheters. This MCP server allows you to calculate the exact amount of yarn required for any project by analyzing gauge, pattern multiples, and dimensions. Use `calculate_single_segment_usage` for individual pieces or `calculate_multi_color_project_summary` to aggregate multiple color segments into a single report. It supports all major yarn weight categories from lace to super bulky.


## Available Tools (3)
- **calculate_multi_color_project_summary**: Calculate summary for multiple segments
- **calculate_single_segment_usage**: Calculate usage for one segment
- **get_yarn_weight_catalog**: Get the yarn weight catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yarn Length Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much yarn do I need for a 20x20cm square in worsted weight with a gauge of 20 stitches and 28 rows per 10cm?"

**🤖 AI Agent:**
> You will need approximately 45.6 meters of worsted weight yarn for this segment.

---

**👤 You:**
> "Calculate the total yarn needed for a blue segment (10x10cm, sport weight, 24 sts/10cm, 32 rows/10cm) and a white segment (15x15cm, sport weight, 24 sts/10cm, 32 rows/10cm)."

**🤖 AI Agent:**
> Total project requirement: 72.5 meters. Breakdown: Blue: 28.8m, White: 43.7m.

---

**👤 You:**
> "What are the consumption constants for different yarn weights?"

**🤖 AI Agent:**
> The yardage per stitch constants are: lace: 0.05, fingering: 0.06, sport: 0.08, dk: 0.1, worsted: 0.12, bulky: 0.15, super_bulky: 0.2.


## ❓ FAQ

**Q: How do I calculate yarn for a project with multiple colors?**
You can use the `calculate_multi_color_project_summary` tool. Simply provide a JSON array containing the details for each color segment, including dimensions and yarn weight.

**Q: What yarn weights are supported?**
The tool supports lace, fingering, sport, dk, worsted, bulky, and super bulky. You can retrieve the exact consumption constants using `get_yarn_weight_catalog`.

**Q: Does it account for pattern repeats?**
Yes. By providing stitch width and height multiples, the calculator adjusts your dimensions to the nearest valid pattern repeat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yarn-length-calculator](https://vinkius.com/mcp/yarn-length-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yarn Length Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yarn-length-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yarn Length Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yarn-length-calculator": {
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
