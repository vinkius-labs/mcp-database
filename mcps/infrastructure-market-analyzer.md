# Infrastructure Market Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infrastructure-market-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Evaluates competitive landscape, concentration, and defensive moats in infrastructure markets.

## Description
This MCP server provides a structural framework to analyze infrastructure markets. It calculates market concentration using HHI, evaluates entry barriers, and assesses competitive intensity. Use `analyze_market_concentration` to identify market types, `evaluate_entry_barriers` to measure moat strength, and `calculate_competitive_intensity` to understand competitive pressure. Finally, `generate_market_summary` synthesizes these metrics into a strategic overview.


## Available Tools (4)
- **analyze_market_concentration**: Determines the concentration level and primary market structure type based on participant count and HHI
- **calculate_competitive_intensity**: Provides a detailed view of how aggressive the competition is within the specific market context
- **evaluate_entry_barriers**: Measures the difficulty for new players to enter the market
- **generate_market_summary**: Synthesizes all previous metrics into a comprehensive strategic overview of the market


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Market Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a market with 3 competitors and an HHI of 2500."

**🤖 AI Agent:**
> The market is classified as an Oligopoly with a high concentration level and high competitive intensity.

---

**👤 You:**
> "What is the entry difficulty if the barrier score is 80 and the regulatory moat is 90?"

**🤖 AI Agent:**
> The entry difficulty is Prohibitive with a Fortified moat strength.

---

**👤 You:**
> "Calculate the intensity for 50 competitors, HHI 500, and an incumbent advantage of 20."

**🤖 AI Agent:**
> The competitive intensity score is high, characterized by a Price-driven nature and minimal incumbent impact.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It provides tools to analyze market concentration, entry barriers, and competitive intensity for infrastructure sectors.

**Q: How do I use the concentration tool?**
You can use `analyze_market_concentration` by providing the competitor count and the HHI value.

**Q: Can I get a full strategic report?**
Yes, by using `generate_market_summary` after running the individual analysis tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infrastructure-market-analyzer](https://vinkius.com/ai-agent-connect/infrastructure-market-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Market Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-market-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Market Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-market-analyzer": {
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
