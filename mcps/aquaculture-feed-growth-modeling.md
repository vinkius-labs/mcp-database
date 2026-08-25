# Aquaculture Feed & Growth Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aquaculture-feed-growth-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict fish growth, feed requirements, and harvest timelines using biological models.

## Description
This MCP server provides specialized modeling for aquaculture management. It uses the Thermal Growth Coefficient (TGC) model to predict how fish weight changes relative to water temperature. Users can calculate expected daily growth, Feed Conversion Ratio (FCR), and total feed requirements. The server also evaluates how environmental factors like dissolved oxygen and temperature impact metabolic efficiency. Key tools include `get_growth_projections` for biomass planning, `evaluate_environmental_impact` for assessing water constraints, and `calculate_harvest_schedule` for predicting harvest dates.


## Available Tools (3)
- **calculate_harvest_schedule**: Calculates the realistic harvest timeline for biomass
- **evaluate_environmental_impact**: Evaluates how water conditions limit feeding efficiency
- **get_growth_projections**: Predicts fish growth trajectories and feed requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aquaculture Feed & Growth Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much feed will I need for 1000kg of Salmon to reach 5kg from 1kg at 12 degrees Celsius?"

**🤖 AI Agent:**
> To grow your Salmon from 1kg to 5kg at 12°C, you will require approximately 4,250kg of feed based on the projected FCR.

---

**👤 You:**
> "What is the impact of low oxygen on my fish metabolism?"

**🤖 AI Agent:**
> At a dissolved oxygen level of 3.5 mg/L, the metabolism multiplier is reduced by 40%, significantly slowing down the growth rate.

---

**👤 You:**
> "When can I harvest my Tilapia if they are currently 200g and I want them to be 500g?"

**🤖 AI Agent:**
> Based on current water conditions, your Tilapia are projected to reach the 500g target weight in approximately 45 days.


## ❓ FAQ

**Q: How does temperature affect the growth predictions?**
The model uses the Thermal Growth Coefficient (TGC) to adjust growth rates based on water temperature, as metabolic rates in fish are temperature-dependent.

**Q: Can I predict when my fish will be ready for harvest?**
Yes, by using the `calculate_harvest_schedule` tool, you can determine the estimated days until harvest based on current weight, target weight, and environmental conditions.

**Q: How does dissolved oxygen impact the results?**
Low dissolved oxygen levels act as a physiological constraint. You can use `evaluate_environmental_impact` to see how oxygen levels reduce metabolic efficiency and growth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aquaculture-feed-growth-modeling](https://vinkius.com/ai-agent-connect/aquaculture-feed-growth-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aquaculture Feed & Growth Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aquaculture-feed-growth-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aquaculture Feed & Growth Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aquaculture-feed-growth-modeling": {
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
