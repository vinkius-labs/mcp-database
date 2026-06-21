# Calorie Deficit Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calorie-deficit-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate BMR, TDEE, and personalized weight loss plans with precision.

## Description
This MCP server provides a specialized toolkit for metabolic planning. Use `compute_bmr` to find your basal metabolic rate, `compute_tdee` to determine daily maintenance calories based on activity, and `calculate_weight_loss_plan` to establish a sustainable caloric deficit. You can also use `estimate_attainment_timeline` to predict how many weeks it will take to reach your target weight.


## Available Tools
- **calculate_weight_loss_plan**: Calculate Weight Loss Plan
- **compute_bmr**: Calculate Basal Metabolic and Metabolic Rate (BMR)
- **compute_tdee**: Calculate Total Daily Energy Expenditure (TDEE)
- **estimate_attainment_timeline**: Estimate Weight Loss Timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calorie Deficit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a 30 year old male, 80kg, 180cm. I am moderately active. How many calories should I eat to lose 0.5kg per week?"

**🤖 AI Agent:**
> Based on your profile, your BMR is approximately 1785 kcal and your TDEE is 2750 kcal. To lose 0.5kg per week, you should target a daily intake of 2375 calories.

---

**👤 You:**
> "How long will it take to go from 100kg to 90kg if I lose 0.5kg per week?"

**🤖 AI Agent:**
> It will take approximately 20 weeks to reach your target weight of 90kg.

---

**👤 You:**
> "Calculate my BMR for a 25 year old female, 60kg, 165cm."

**🤖 AI Agent:**
> Your Basal Metabolic Rate (BMR) is approximately 1385 calories per day.


## ❓ FAQ

**Q: How do I calculate my maintenance calories?**
First, use `compute_bmr` with your age, weight, height, and sex. Then, take that result and pass it to `compute_tdee` along with your physical activity level.

**Q: Can I plan for a specific weight loss goal?**
Yes. Use `calculate_weight_loss_plan` by providing your TDEE and your desired weekly weight loss amount to find your target daily calorie intake.

**Q: Does the calculator support both metric and imperial units?**
Yes, all tools allow you to specify a `unitSystem` as either 'metric' or 'imperial'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calorie-deficit-calculator](https://vinkius.com/mcp/calorie-deficit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calorie Deficit Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calorie-deficit-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calorie Deficit Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calorie-deficit-calculator": {
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
