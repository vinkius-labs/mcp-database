# Calorie Burn Estimator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calorie-burn-estimator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/calorie-burn-estimator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/calorie-burn-estimator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate energy expenditure using MET values, body weight, and activity duration.

## Description
The Calorie Burn Estimator MCP server provides a precise way to calculate calories burned during physical activities. By using the Metabolic Equivalent of Task (MET) principle, it calculates energy expenditure based on your body weight and the duration of the exercise. You can use `search_activities` to find specific exercises in our database of over 80 activities, `estimate_calories_burned` to get exact calorie counts, and `classify_activity_intensity` to understand the physiological effort level of an activity.


## Available Tools
- **classify_activity_intensity**: Classify the intensity of an activity
- **estimate_calories_burned**: Estimate calories burned during an activity
- **search_activities**: Search for physical activities and their MET values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calorie Burn Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories do I burn if I run for 30 minutes at a weight of 70kg?"

**🤖 AI Agent:**
> Running (assuming a MET of 9.8) for 30 minutes at 70kg burns approximately 228.67 calories.

---

**👤 You:**
> "Find me some low intensity activities."

**🤖 AI Agent:**
> Some low intensity activities include walking, stretching, and light yoga.

---

**👤 You:**
> "What is the intensity level of an activity with a MET value of 7?"

**🤖 AI Agent:**
> An activity with a MET value of 7 is classified as Moderate Intensity.


## Installation & Usage

To install and use the **Calorie Burn Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calorie-burn-estimator](https://vinkius.com/mcp/calorie-burn-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
