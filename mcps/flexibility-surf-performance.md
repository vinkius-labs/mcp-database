# Flexibility Surf Performance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flexibility-surf-performance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [performance](../categories/performance.md)

Assess how joint mobility impacts surfing maneuvers and performance.

## Description
This MCP server provides a physiological assessment engine for surfers. By analyzing hip mobility, thoracic rotation, and ankle flexibility, it calculates a holistic flexibility score and identifies specific movement limitations. Use `analyze_flexibility` to get a baseline assessment, `evaluate_maneuver_readiness` to check capability for specific moves like bottom turns or aerials, and `get_performance_impact_summary` to understand how mobility constraints affect overall surfing performance.


## Available Tools (4)
- **analyze_flexibility**: Calculates the overall flexibility score and identifies specific movement limitations
- **compare_mobility_tiers**: Compares a user's metrics against standardized performance tiers
- **evaluate_maneuver_readiness**: Determines how well a surfer can perform specific surfing maneuvers
- **get_performance_impact_summary**: Provides a high-level overview of how mobility constraints translate to surfing performance gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flexibility Surf Performance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my flexibility with hip mobility 45, thoracic rotation 30, and ankle flexibility 40."

**🤖 AI Agent:**
> Your flexibility score is 38. Your primary constraint is thoracic rotation, which may limit your ability to perform high-velocity carves.

---

**👤 You:**
> "How ready am I for an aerial if my hip mobility is 50, thoracic rotation 45, and ankle flexibility 45?"

**🤖 AI Agent:**
> Your readiness score for an aerial is 85. You have sufficient mobility to manage board orientation during flight.

---

**👤 You:**
> "What is my performance impact summary for a flexibility score of 60 and limitations: ['limited hip mobility']?"

**🤖 AI Agent:**
> Your performance level is Intermediate. The impact severity is Moderate. Focus on hip mobility exercises to improve bottom turn depth.


## ❓ FAQ

**Q: How do I use this to improve my surfing?**
Use `analyze_flexibility` to identify your primary constraints, then use `evaluate_maneuver_readiness` to see how those constraints specifically limit maneuvers like carves or aerials.

**Q: What metrics are required for the analysis?**
The engine requires three specific metrics: hip mobility, thoracic rotation, and ankle flexibility.

**Q: Can I check my readiness for specific maneuvers?**
Yes, the `evaluate_maneuver_readiness` tool allows you to check your capability for bottom turns, carves, and aerials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flexibility-surf-performance](https://vinkius.com/en/ai-agent-connect/flexibility-surf-performance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flexibility Surf Performance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flexibility-surf-performance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flexibility Surf Performance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flexibility-surf-performance": {
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
