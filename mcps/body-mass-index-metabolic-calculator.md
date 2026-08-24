# Body Mass Index & Metabolic Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/body-mass-index-metabolic-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate BMI, BMR, TDEE, and macronutrient needs for metabolic health.

## Description
This MCP server provides precise physiological metrics for weight management and metabolic health analysis. Using the `calculate_body_metrics` tool, AI agents can determine a user's Body Mass Index (BMI), Basal Metabolic Rate (BMR) via the Mifflin-St Jeor equation, and Total Daily Energy Expenditure (TDEE). It also calculates ideal weight ranges using the Devine formula and provides a specific macronutrient split for weight maintenance. You can also use `get_activity_factors` to see metabolic multipliers or `get_bmi_thresholds` to understand weight category ranges.


## Available Tools (3)
- **get_bmi_thresholds**: Provides the BMI numerical ranges for each weight category
- **calculate_body_metrics**: Provides a comprehensive overview of a user's current physical status and metabolic needs
- **get_activity_factors**: Provides the multipliers used to convert BMR into TDEE


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Body Mass Index & Metabolic Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my body metrics. I am a 30-year-old male, 85kg, 180cm, with a moderate activity level."

**🤖 AI Agent:**
> Your BMI is 26.2 (Overweight). Your BMR is 1,845 calories, and your TDEE is 2,830 calories. Your ideal weight range is 67-83 kg. For maintenance, you need 170g of protein, 78g of fat, and 345g of carbs.

---

**👤 You:**
> "What are the BMI thresholds for weight categories?"

**🤖 AI Agent:**
> The standard BMI categories are: Underweight (below 18.5), Normal (18.5-24.9), Overweight (25-29.9), and Obese (30 or above).

---

**👤 You:**
> "What activity multipliers are used for TDEE?"

**🤖 AI Agent:**
> The multipliers are: sedentary, light, moderate, active, and very_active.


## ❓ FAQ

**Q: What metrics does this server provide?**
The server provides BMI, BMI category, BMR, TDEE, ideal weight range, and a macronutrient split for weight maintenance.

**Q: How is the BMR calculated?**
BMR is calculated using the Mifflin-St Jeor equation, which is a standard method for estimating metabolic rate.

**Q: Can I use this for weight maintenance planning?**
Yes, the tool calculates a specific macronutrient split (protein, fats, and carbs) designed for weight maintenance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/body-mass-index-metabolic-calculator](https://vinkius.com/ai-agent-connect/body-mass-index-metabolic-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Body Mass Index & Metabolic Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `body-mass-index-metabolic-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Body Mass Index & Metabolic Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "body-mass-index-metabolic-calculator": {
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
