# Enterprise Champion Identification Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-champion-identification-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-analytics](../categories/sales-analytics.md)

Analyze sales efficacy by measuring champion identification success, impact on win rates, and identification velocity.

## Description
This MCP server provides a performance analytics engine to evaluate how effectively sales teams identify and leverage key decision-makers. By connecting your AI agent to these tools, you can calculate the `analyze_identification_success` rate to see how many deals have verified champions, use `calculate_champion_impact` to determine the lift in win probability, and track `measure_identification_velocity` to monitor the speed of discovery. It also includes `evaluate_champion_effectiveness` to assess how well resources are enabling stakeholders to advocate for your solution.


## Available Tools (4)
- **analyze_identification_success**: Answers how successful the team is at identifying champions in the current pipeline
- **calculate_champion_impact**: Answers how much having a champion increases the chances of winning
- **evaluate_champion_effectiveness**: Answers how well champions are being enabled to advocate for the solution
- **measure_identification_velocity**: Answers how quickly champions are being found in sales cycles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Champion Identification Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current champion identification rate if we have 50 total deals and 30 have verified champions?"

**🤖 AI Agent:**
> The current champion identification rate is 60%.

---

**👤 You:**
> "How much did having a champion increase our win rate? We had 20 deals with champions (15 won) and 20 deals without champions (5 won)."

**🤖 AI Agent:**
> Having a champion increased the win rate from 25% to 75%, resulting in a significant impact lift.

---

**👤 You:**
> "How fast are we finding champions? We spent a total of 150 days identifying champions across 10 deals."

**🤖 AI Agent:**
> The average time to identify a champion is 15 days.


## ❓ FAQ

**Q: How do I calculate the impact of a champion on my win rate?**
You can use the `calculate_champion_impact` tool. Provide the number of deals with and without champions, along with their respective win counts, to see the relative lift in win probability.

**Q: What does identification velocity tell me?**
Identification velocity, measured via `measure_identification_velocity`, tracks the average number of days it takes to find a champion. Faster identification is a leading indicator of healthy deal progression.

**Q: Can I assess how well I am supporting my champions?**
Yes, the `evaluate_champion_effectiveness` tool calculates a composite index based on your enablement score and the champion's influence level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-champion-identification-rate](https://vinkius.com/ai-agent-connect/enterprise-champion-identification-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Champion Identification Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-champion-identification-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Champion Identification Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-champion-identification-rate": {
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
