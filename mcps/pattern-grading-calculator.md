# Pattern Grading Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pattern-grading-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Scale sewing patterns between sizes using ASTM standards (Women, Men, Children).

## Description
The Pattern Grading Calculator automates the mathematical process of enlarging or reducing garment patterns. By applying industry-standard ASTM rules (D5585 for Women, D6458 for Men, and D6192 for Children), it calculates precise grade rules for various anatomical landmarks. Use `calculate_standard_increment` to find total circumference changes, `distribute_size_increments` to split growth between bust, waist, and hip, or `compute_pattern_grading_table` to generate a complete measurement difference table for any target size.


## Available Tools (3)
- **compute_pattern_grading_table**: Generates a complete table showing how much every individual pattern point should move for a specific target size
- **distribute_size_increments**: Splits a total circumference change into specific, usable increments for key body landmarks
- **calculate_standard_increment**: Determines the total amount of circumference change required for a single size jump within a chosen standard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pattern Grading Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total circumference change should I expect for 2 size jumps in the Women's standard?"

**🤖 AI Agent:**
> For a 2-size jump using the Women's ASTM standard, the total cumulative change in circumference is 5.0 units.

---

**👤 You:**
> "If I have a total change of 6cm to distribute, how much goes to the waist?"

**🤖 AI Agent:**
> Using standard distribution, the 6cm change is split into 2cm for the bust, 2cm for the waist, and 2cm for the hip.

---

**👤 You:**
> "Generate a grading table for a target size of 1 jump up from base measurements: {'bust': 90, 'waist': 70, 'hip': 95} using Men's standard."

**🤖 AI Agent:**
> The generated grade table shows an increase of 2.5cm for the bust, waist, and hip landmarks, with corresponding shifts for neck and armscye points.


## ❓ FAQ

**Q: What industry standards does this tool use?**
The tool follows ASTM D5585 for Women, D6458 for Men, and D6192 for Children to ensure consistent fit across sizes.

**Q: How is the circumference change distributed?**
Using the `distribute_size_increments` tool in 'Standard' mode, the total change is split equally (1/3 each) between the bust, waist, and hip measurements.

**Q: Can I generate a full table for all pattern points?**
Yes, by using `compute_pattern_grading_table`, you can provide base measurements and a target size to receive a complete list of grade rules for landmarks like neck, armscye, and shoulder.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pattern-grading-calculator](https://vinkius.com/mcp/pattern-grading-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pattern Grading Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pattern-grading-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pattern Grading Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pattern-grading-calculator": {
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
