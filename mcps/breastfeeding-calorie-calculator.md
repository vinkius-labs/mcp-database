# Breastfeeding Calorie Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/breastfeeding-calorie-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates caloric, hydration, and nutritional needs for lactating individuals.

## Description
This MCP server provides specialized tools to manage nutritional requirements during lactation. It calculates total daily energy needs, hydration targets, and safe weight loss boundaries. Use `get_lactation_requirements` to get a full overview of caloric and hydration needs, or `get_energy_cost_summary` to see the breakdown between basal metabolic rate, activity expenditure, and lactation energy cost. It also includes `get_weight_management_safety` to ensure caloric intake remains within safe limits for milk production.


## Available Tools (4)
- **get_weight_management_safety**: Determines the nutritional safety boundaries for individuals attempting to manage weight during lactation
- **get_energy_cost_summary**: Breaks down where the energy is being used (Basal vs. Activity vs. Lactation)
- **get_hydration_guidelines**: Calculates specific fluid intake targets and provides context on hydration needs
- **get_lactation_requirements**: Provides a comprehensive overview of caloric and hydration needs based on the current lactation status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breastfeeding Calorie Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 3 weeks postpartum, breastfeeding exclusively, and weigh 65kg. I have a moderate activity level and feed 8 times a day. What are my daily needs?"

**🤖 AI Agent:**
> Your total daily caloric requirement is 2,450 calories, with an additional 500 calories specifically for milk production. You should aim for approximately 3.2 liters of water daily to maintain hydration.

---

**👤 You:**
> "How much water should I drink if I feed my baby 10 times a day and am exclusively breastfeeding?"

**🤖 AI Agent:**
> Based on a feeding frequency of 10 times per day and exclusive breastfeeding, your recommended daily fluid intake is 3.5 liters.

---

**👤 You:**
> "I need to lose weight safely. My total daily calories are 2200 and I am breastfeeding exclusively. What is my safe deficit?"

**🤖 AI Agent:**
> To protect your milk supply, your minimum safe caloric intake is 1,850 calories. Your recommended daily deficit for gradual weight loss is 350 calories.


## ❓ FAQ

**Q: How does this tool help with weight loss?**
The tool uses `get_weight_management_safety` to determine a safe caloric deficit that supports milk production while allowing for gradual weight management.

**Q: Can I calculate my hydration needs?**
Yes, you can use `get_hydration_guidelines` to find your recommended daily fluid intake based on feeding frequency.

**Q: Does it account for different activity levels?**
Yes, the `get_lactation_requirements` tool accepts activity levels such as sedentary, moderate, or active to adjust energy expenditure calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/breastfeeding-calorie-calculator](https://vinkius.com/en/ai-agent-connect/breastfeeding-calorie-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breastfeeding Calorie Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breastfeeding-calorie-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breastfeeding Calorie Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breastfeeding-calorie-calculator": {
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
