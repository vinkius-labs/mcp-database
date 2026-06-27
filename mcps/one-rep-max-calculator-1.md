# One-Rep Max Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/one-rep-max-calculator-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate your maximum strength capacity using 8 different physiological models.

## Description
The One-Rep Max Calculator provides a comprehensive analysis of your lifting potential. By inputting the weight lifted and repetitions performed, you can use `calculate_all_1rm_formulas` to see estimates from eight distinct models: Epley, Brzycki, Lander, Lombardi, Mayhew, O'Conner, Wathan, and the mean of all. This tool helps identify your strength baseline without the physical risk of a true 1RM test. Additionally, use `get_perc_table` to generate training intensity charts from 50% to 100%, and `identify_best` to find the most accurate formula for your current repetition range.


## Available Tools (3)
- **calculate_all_1rm_formulas**: Calculates the theoretical 1RM using all eight distinct estimation models
- **get_perc_table**: Generates a training intensity reference table
- **identify_best**: Recommends the most reliable estimation formula


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One-Rep Max Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just lifted 100kg for 5 reps. What is my estimated 1RM using all formulas?"

**🤖 AI Agent:**
> Based on your 100kg lift for 5 reps, the Epley estimate is 120kg, Brzycki is 116.67kg, and the average across all eight models is approximately 118.45kg.

---

**👤 You:**
> "Generate a training table for a 120kg 1RM."

**🤖 AI Agent:**
> For a 120kg baseline, your 50% target is 60kg, 75% is 90kg, and 100% is 120kg.

---

**👤 You:**
> "I did 8 reps recently. Which formula is best for me?"

**🤖 AI Agent:**
> For a set of 8 repetitions, the Wathan model is recommended as it accounts for higher volume fatigue factors.


## ❓ FAQ

**Q: How accurate are these 1RM estimates?**
Accuracy depends on your repetition range. Low repetitions (1-3) provide the most reliable data across all models, while higher reps may lead to slight variations between formulas.

**Q: Which formula should I use?**
You can use the `identify_best` tool to automatically receive a recommendation based on your recent repetition count.

**Q: Can I generate training percentages?**
Yes, by using `get_perc_table` with your estimated 1RM, you can generate a detailed table of target weights from 50% to 100%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/one-rep-max-calculator-1](https://vinkius.com/mcp/one-rep-max-calculator-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **One-Rep Max Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `one-rep-max-calculator-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **One-Rep Max Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "one-rep-max-calculator-1": {
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
