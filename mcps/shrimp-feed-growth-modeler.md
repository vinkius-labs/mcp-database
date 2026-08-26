# Shrimp Feed & Growth Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/shrimp-feed-growth-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predictive modeling for shrimp growth, feed requirements, and survival risk.

## Description
This MCP server provides advanced predictive modeling for shrimp aquaculture. It connects AI agents to biological and environmental data to calculate growth trajectories, feed efficiency, and harvest timelines. Using `get_growth_projection`, agents can estimate harvest dates and final biomass. The `calculate_feed_requirements` tool determines daily feed needs, while `estimate_survival_and_risk` assesses health threats based on water parameters. Finally, `analyze_pond_efficiency` compares real-world performance against species-specific biological optima.


## Available Tools (4)
- **analyze_pond_efficiency**: Compares current growth and feed performance against theoretical species optima
- **calculate_feed_requirements**: Determines the amount of feed needed to sustain growth
- **estimate_survival_and_risk**: Evaluates the likelihood of shrimp survival and potential disease impact
- **get_growth_projection**: Predicts the growth trajectory, expected harvest date, and final biomass


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shrimp Feed & Growth Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days until my L. vannamei reach 20g if I have 500kg of biomass and the water is 28°C?"

**🤖 AI Agent:**
> Based on the current parameters, it will take approximately 45 days to reach the target weight, with an estimated final biomass of 520kg.

---

**👤 You:**
> "What is the daily feed requirement for 1000kg of P. monodon at 26°C?"

**🤖 AI Agent:**
> The daily feed requirement for 1000kg of biomass is 25.5kg, with a predicted FCR of 1.4.

---

**👤 You:**
> "Assess the survival risk for my pond with 25°C temperature and medium management intensity."

**🤖 AI Agent:**
> The predicted survival rate is 85% with a low disease risk score.


## ❓ FAQ

**Q: Which shrimp species are supported?**
The model currently supports L. vannamei (Whiteleg shrimp) and P. monodon (Giant tiger prawn).

**Q: How accurate are the growth projections?**
Projections are based on temperature-dependent growth models and species-specific metabolic constants, providing a scientific estimate of biomass and harvest dates.

**Q: Can I use this to manage feed costs?**
Yes, by using `calculate_feed_requirements`, you can determine the exact amount of feed needed for the current biomass to optimize efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/shrimp-feed-growth-modeler](https://vinkius.com/ai-agent-connect/shrimp-feed-growth-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shrimp Feed & Growth Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shrimp-feed-growth-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shrimp Feed & Growth Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shrimp-feed-growth-modeler": {
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
