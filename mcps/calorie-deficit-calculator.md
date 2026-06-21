# Calorie Deficit Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calorie-deficit-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/calorie-deficit-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/calorie-deficit-calculator-mcp)
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


## Installation & Usage

To install and use the **Calorie Deficit Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calorie-deficit-calculator](https://vinkius.com/mcp/calorie-deficit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
