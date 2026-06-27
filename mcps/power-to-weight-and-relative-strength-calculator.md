# Power-to-Weight and Relative Strength Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/power-to-weight-and-relative-strength-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate W/kg for endurance sports and standardized strength scores (DOTS, WILKS, IPF) for powerlifting.

## Description
This MCP server provides a specialized performance metric engine for quantifying power output per kilogram in endurance sports and standardized relative strength scores in weightlifting. Use `calculate_wkg_ratio` to determine Watts per Kilogram (W/kg) for cycling and CrossFit, or `calculate_relative_strength` to compute DOTS, WILKS, or IPF points for powerlifting. You can also use `get_performance_rank` to categorize your performance into tiers like Elite, Advanced, or Intermediate by comparing your metrics against professional benchmarks.


## Available Tools (3)
- **calculate_wkg_ratio**: Calculates the power-to-weight ratio (W/kg) for endurance sports
- **get_performance_rank**: Categorizes an athlete's performance into a tier
- **calculate_relative_strength**: Computes standardized relative strength scores for powerlifting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Power-to-Weight and Relative Strength Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my W/kg ratio if I weigh 75kg and can produce 300 Watts."

**🤖 AI Agent:**
> Your power-to-weight ratio is 4.0 W/kg.

---

**👤 You:**
> "What is my DOTS score if I weigh 90kg and my total lift (S+B+D) is 250kg?"

**🤖 AI Agent:**
> Your calculated DOTS score is approximately 345.2.

---

**👤 You:**
> "Is a 5.0 W/kg ratio considered elite in cycling?"

**🤖 AI Agent:**
> A 5.0 W/kg ratio is categorized as Elite performance in cycling, placing you among the world's top professional athletes.


## ❓ FAQ

**Q: What is the Power-to-Weight ratio (W/kg)?**
It is a metric used in endurance sports like cycling to compare power output relative to body mass. It is calculated by dividing Watts by Kilograms.

**Q: Which scoring systems are supported for powerlifting?**
The tool supports DOTS, WILKS, and IPF points to normalize strength across different weight classes.

**Q: How can I see my performance tier?**
Use the `get_performance_rank` tool with your calculated metric value and sport type to see if you fall into Elite, Advanced, Intermediate, or Novice categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/power-to-weight-and-relative-strength-calculator](https://vinkius.com/mcp/power-to-weight-and-relative-strength-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Power-to-Weight and Relative Strength Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `power-to-weight-and-relative-strength-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Power-to-Weight and Relative Strength Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "power-to-weight-and-relative-strength-calculator": {
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
