# Gut Health Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gut-health-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess your digestive health with detailed gut scores and dietary insights.

## Description
This MCP server provides a comprehensive assessment of your digestive wellness. By analyzing dietary habits and physiological indicators, it uses tools like `calculate_gut_score` to provide a holistic health score, identify risk factors, and offer specific dietary recommendations. You can also use `analyze_transit_health` to evaluate intestinal movement via the Bristol Stool Scale, `evaluate_dietary_impact` to check nutritional balance, and `identify_risk_factors` to pinpoint threats to gut stability.


## Available Tools (4)
- **analyze_transit_health**: Evaluates the efficiency of intestinal movement based on stool consistency
- **calculate_gut_score**: Provides a holistic assessment of an individual's current gut health status
- **evaluate_dietary_impact**: Specifically examines the relationship between fiber, fermentation, and hydration
- **identify_risk_factors**: Isolates and describes the primary threats to gut stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gut Health Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my gut health score. I eat 30g of fiber, 3 servings of fermented foods a week, drink 2 liters of water, haven't used antibiotics recently, have no symptoms, and my Bristol scale type is 4."

**🤖 AI Agent:**
> Your gut health score is 85/100. Your digestive system is in an optimal state with healthy transit and balanced nutrition.

---

**👤 You:**
> "Check my transit health. My Bristol scale type is 2."

**🤖 AI Agent:**
> Your transit status is Slow. You may need to increase your water intake and fiber consumption to improve regularity.

---

**👤 You:**
> "What are my primary gut health risks? I recently took antibiotics and I am experiencing bloating."

**🤖 AI Agent:**
> Your primary risks are recent antibiotic use and gastrointestinal symptoms, resulting in a High severity level for gut stability.


## ❓ FAQ

**Q: How accurate is the gut health score?**
The score is a composite metric based on the dietary and physiological data you provide, such as fiber intake and Bristol Scale types.

**Q: Can I use this to track my fiber intake?**
Yes, you can use `evaluate_dietary_impact` to see how your fiber, fermentation, and hydration levels affect your nutritional balance.

**Q: What is the Bristol Stool Scale?**
It is a standardized medical tool used to classify stool consistency, which helps the tool determine your transit health status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gut-health-score](https://vinkius.com/en/ai-agent-connect/gut-health-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gut Health Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gut-health-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gut Health Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gut-health-score": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
