# Accelerator Thematic Performance Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-thematic-performance-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze investment efficacy across industry verticals and thematic focuses.

## Description
This MCP server provides specialized analytical tools for venture accelerators to evaluate portfolio performance. It calculates capital efficiency, identifies optimal industry themes based on risk tolerance, and assesses portfolio concentration risk to prevent over-exposure to specific sectors. Use `get_vertical_performance` to compare sector metrics, `identify_best_themes` to find the best balance of risk and reward, and `analyze_concentration_risk` to monitor vulnerability to market cycles.


## Available Tools (3)
- **analyze_concentration_risk**: Am I too heavily invested in one area, and how vulnerable am I to sector-specific market crashes?
- **get_vertical_performance**: How is each industry vertical performing according to my investment metrics?
- **identify_best_themes**: Which specific industry themes are providing the most optimal balance of risk and reward?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Thematic Performance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is each industry vertical performing according to my investment metrics?"

**🤖 AI Agent:**
> The Fintech vertical shows a capital efficiency of 1.2 and a survival rate of 85%, while HealthTech has a survival rate of 92% with lower exit volume.

---

**👤 You:**
> "Which specific industry themes are providing the most optimal balance of risk and reward?"

**🤖 AI Agent:**
> Based on your risk tolerance, the AI identifies SaaS and CleanTech as the top-performing themes with the highest performance scores.

---

**👤 You:**
> "Am I too heavily invested in one area, and how vulnerable am I to sector-specific market crashes?"

**🤖 AI Agent:**
> Your concentration in AI is High, with 45% of total capital and 50% of entities, indicating significant vulnerability to sector-specific downturns.


## ❓ FAQ

**Q: How does the engine calculate capital efficiency?**
Capital efficiency is determined by the ratio of exit success density relative to the total capital deployed within a specific vertical.

**Q: Can I adjust the analysis based on my risk appetite?**
Yes, by using `identify_best_themes`, you can provide a risk tolerance weight between 0 and 1 to prioritize either survival rates or exit volume.

**Q: How is concentration risk identified?**
The `analyze_concentration_risk` tool evaluates both capital and entity concentration. If a vertical exceeds established thresholds, it is flagged with a High risk level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-thematic-performance-engine](https://vinkius.com/ai-agent-connect/accelerator-thematic-performance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Thematic Performance Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-thematic-performance-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Thematic Performance Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-thematic-performance-engine": {
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
