# Metabolic Energy Estimator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metabolic-energy-estimator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/metabolic-energy-estimator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/metabolic-energy-estimator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Empower your AI Agent with deterministic metabolic calculations. Estimate burned calories with a local catalog of 80+ activities, calculate TDEE, and project weight loss timelines.

## Description
Autonomous health and fitness agents demand uncompromising metabolic accuracy. When standard LLMs attempt to estimate calories burned for a specific activity, they guess wildly. The Metabolic Energy Estimator MCP empowers your AI Agent by delegating this logic to a deterministic engine utilizing scientifically validated MET (Metabolic Equivalent of Task) values.

### Core Capabilities
- **Agentic Calorie Estimation:** Search a native, offline catalog of over 80 specific physical activities and calculate exact calories burned based on the user's exact weight and duration.
- **TDEE & BMR Engine:** Implements the rigorous Mifflin-St Jeor equation to establish the user's Basal Metabolic Rate and Total Daily Energy Expenditure without sending health metrics to the cloud.
- **Weight Loss Projection:** Compute the exact number of days and weeks required to hit a target weight given a precise daily caloric deficit, complete with safety warnings.


## Available Tools
- **calculate_tdee**: Calculates Total Daily Energy Expenditure (TDEE) and Basal Metabolic Rate (BMR) using the Mifflin-St Jeor equation
- **estimate_calories_burned**: You MUST provide an activityId found via search_activity_catalog.

Calculates exactly how many calories are burned doing a specific physical activity based on weight and time
- **search_activity_catalog**: Searches the deterministic local catalog for activities and their exact MET values
- **calculate_weight_loss_projection**: 1kg of fat = 7700 calories.

Projects how many days and weeks it will take to reach a target weight based on a daily calorie deficit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metabolic Energy Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 80kg and ran moderately for 45 minutes. How many calories did I burn?"

**🤖 AI Agent:**
> Using the search_activity_catalog and estimate_calories_burned tools: The activity 'run_moderate' has a MET of 9.8. You burned approximately 588 calories.

---

**👤 You:**
> "I am a 30-year-old male, 180cm, 85kg, with a sedentary lifestyle. What is my TDEE?"

**🤖 AI Agent:**
> Using the calculate_tdee tool: Your BMR is 1830 kcal/day and your Total Daily Energy Expenditure (TDEE) is roughly 2196 kcal/day.

---

**👤 You:**
> "I weigh 90kg and want to reach 80kg with a 500 calorie daily deficit. How long will it take?"

**🤖 AI Agent:**
> Using the calculate_weight_loss_projection tool: To lose 10kg, you need to burn 77,000 calories. At a 500/day deficit, it will take exactly 154 days (22 weeks).


## Installation & Usage

To install and use the **Metabolic Energy Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metabolic-energy-estimator](https://vinkius.com/mcp/metabolic-energy-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
