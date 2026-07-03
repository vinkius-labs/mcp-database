# Reverse Diet Metabolism Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reverse-diet-metabolism-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Design a controlled, week-by-week calorie increase plan to restore metabolic health and minimize fat gain.

## Description
The Reverse Diet Metabolism Builder is a specialized simulation engine designed for individuals transitioning from a calorie deficit back to maintenance. By using tools like `generate_reverse_diet_schedule`, you can create an adaptive roadmap that increments calories weekly while monitoring weight gain. The system uses the 7700 kcal rule to estimate mass changes and automatically pauses increases if simulated weight gain exceeds 0.5kg in a four-week window. Additionally, use `predict_weight_impact` to forecast long-term weight trends based on surplus, or `classify_nutritional_state` to identify your current phase, such as `aggressive_deficit` or `maintenance`.


## Available Tools (3)
- **generate_reverse_diet_schedule**: 5kg in 4 weeks.

Generates a week-by-week roadmap for reversing a diet
- **predict_weight_impact**: Estimates weight change based on caloric surplus
- **classify_nutritional_state**: Classifies the current nutritional phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reverse Diet Metabolism Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a reverse diet schedule starting at 1500 calories, targeting 2500 maintenance, with a 50 calorie weekly increase."

**🤖 AI Agent:**
> Your schedule starts at 1500 kcal. Week 1: 1550 kcal, Week 2: 1600 kcal, Week 3: 1650 kcal. The simulation will continue until 2500 kcal is reached, pausing if weight gain exceeds 0.5kg in any 4-week period.

---

**👤 You:**
> "If I eat 2800 calories while my maintenance is 2500 for 30 days, how much weight will I gain?"

**🤖 AI Agent:**
> Based on a daily surplus of 300 calories over 30 days, your estimated weight change is approximately 1.17kg.

---

**👤 You:**
> "I am eating 1800 calories and my maintenance is 2400. What is my current nutritional state?"

**🤖 AI Agent:**
> You are currently in the `moderate_deficit` phase.


## ❓ FAQ

**Q: How does the calorie increase schedule work?**
The `generate_reverse_</sub>diet_schedule` tool iterates week by week, adding your specified increment to your daily calories. If the simulation detects that weight gain is too rapid (over 0.5kg in a rolling 4-week period), it will pause the increase for one week.

**Q: Can I predict how much weight I might gain?**
Yes, you can use the `predict_weight_impact` tool. By providing your current daily calories and maintenance level, it calculates estimated weight change using the 7700 kcal rule.

**Q: How do I know if I am in a deficit or surplus?**
The `classify_nutritional_state` tool compares your current intake to your maintenance target and labels you as being in an `aggressive_deficit`, `moderate_deficit`, `maintenance`, or `surplus` phase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reverse-diet-metabolism-builder](https://vinkius.com/mcp/reverse-diet-metabolism-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reverse Diet Metabolism Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reverse-diet-metabolism-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reverse Diet Metabolism Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reverse-diet-metabolism-builder": {
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
