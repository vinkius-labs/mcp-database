# Sunflower Hybrid Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sunflower-hybrid-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Select optimal sunflower hybrids using multi-criteria analysis of yield, oil, and disease resistance.

## Description
This MCP server provides advanced decision support for sunflower cultivation. It allows AI agents to evaluate hybrid performance by balancing commercial goals with agronomic constraints. Users can use `get_available_hybrids` to browse compatible varieties, `analyze_hybrid_suitability` to calculate specific metrics like expected oil yield, or `select_optimal_hybrid` to perform a weighted multi-criteria analysis. The tool accounts for target markets (oil, confection, bird food), maturity windows, disease pressure (such as downy mildew or sclerotinia), and herbicide resistance traits like Clearfield or ExpressSun.


## Available Tools (3)
- **analyze_hybrid_suitability**: Calculates the specific performance metrics for a single hybrid based on user goals
- **get_available_hybrids**: Provides a list of all sunflower hybrids available in the system to check their baseline characteristics
- **select_optimal_hybrid**: Performs a multi-criteria weighted analysis to recommend the best hybrid for a specific field scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sunflower Hybrid Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which sunflower hybrids are available for the oil market?"

**🤖 AI Agent:**
> The available oil-market hybrids are H-102, H-205, and H-309.

---

**👤 You:**
> "Find the best hybrid for a high-yield oil target with high disease pressure."

**🤖 AI Agent:**
> The recommended hybrid is H-402, which provides the best balance of yield and disease resistance for your specific criteria.

---

**👤 You:**
> "What is the expected oil yield for hybrid H-102 if I target 3000 kg/ha?"

**🤖 AI Agent:**
> For a target yield of 3000 kg/ha, the expected oil yield for H-102 is 540 kg/ha based on its 18% oil content.


## ❓ FAQ

**Q: How do I find hybrids suitable for the oil market?**
You can use the `get_available_hybrids` tool and specify 'oil' as the market type to see all compatible varieties.

**Q: Can I account for herbicide resistance in my selection?**
Yes, when using `select_optimal_hybrid`, you can provide a `requiredHerbicideTrait` to filter for hybrids with specific resistance like Clearfield.

**Q: How is the best hybrid determined?**
The `select_optimal_hybrid` tool uses a weighted scoring system where you define the importance of yield, oil content, and disease resistance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sunflower-hybrid-selector](https://vinkius.com/ai-agent-connect/sunflower-hybrid-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sunflower Hybrid Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sunflower-hybrid-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sunflower Hybrid Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sunflower-hybrid-selector": {
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
