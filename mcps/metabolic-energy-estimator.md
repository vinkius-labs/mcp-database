# Metabolic Energy Estimator MCP Server

Empower your AI Agent with deterministic metabolic calculations. Estimate burned calories with a local catalog of 80+ activities, calculate TDEE, and project weight loss timelines.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/metabolic-energy-estimator)

## Overview
**Category:** data-analytics
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Metabolic Energy Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metabolic-energy-estimator](https://vinkius.com/mcp/metabolic-energy-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
