# Cold Water Survival Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cold-water-survival-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Estimates survival time, hypothermia onset, and swim failure in cold water.

## Description
This MCP server provides critical physiological modeling for cold water immersion. It calculates survival milestones including total survival time, the onset of hypothermia, and the point of swim failure. Users can use `get_survival_estimates` to model specific individuals based on weight, body fat, and wetsuit thickness, or `get_risk_level` to assess immediate danger. The tool also allows for comparing different survival scenarios and evaluating the protective impact of neoprene insulation.


## Available Tools (4)
- **compare_scenarios**: Compares two different physiological or environmental setups to see which provides more survival time
- **get_insulation_impact**: Evaluates how much the wetsuit thickness mitigates heat loss compared to no suit
- **get_risk_level**: Categorizes the immediate danger level based on water temperature and insulation
- **get_survival_estimates**: Calculates all critical survival milestones for a specific individual in specific water conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cold Water Survival Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate survival for a 75kg person with 15% body fat in 10°C water wearing a 5mm wetsuit."

**🤖 AI Agent:**
> The estimated survival time is 4.2 hours, with hypothermia onset at 1.5 hours and swim failure at 2.1 hours.

---

**👤 You:**
> "What is the risk level for 4°C water without a wetsuit?"

**🤖 AI Agent:**
> The risk category is Extreme with a high urgency score.

---

**👤 You:**
> "Compare a 90kg person with 25% body fat in 5°C water to a 70kg person with 10% body fat in the same conditions."

**🤖 AI Agent:**
> The 90kg person with 25% body fat will have a longer survival time due to higher thermal inertia and insulation.


## ❓ FAQ

**Q: How does body fat affect survival estimates?**
Higher body fat percentages provide more natural insulation, which slows the rate of heat loss and extends the estimated survival time.

**Q: Can I include wetsuit thickness in my calculations?**
Yes, you can use `get_survival_estimates` or `get_risk_level` with the `wetsuitThickness` parameter to account for neoprene insulation.

**Q: What is the difference between hypothermia onset and swim failure?**
Hypothermia onset is when core temperature begins to drop below normal, while swim failure is the point where muscle coordination is lost, making movement impossible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cold-water-survival-estimator](https://vinkius.com/en/ai-agent-connect/cold-water-survival-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cold Water Survival Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cold-water-survival-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cold Water Survival Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cold-water-survival-estimator": {
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
