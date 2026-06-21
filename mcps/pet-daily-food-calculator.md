# Pet Daily Food Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-daily-food-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pet-daily-food-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pet-daily-food-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise daily food portions and feeding schedules for your dog based on weight, life stage, and activity level.

## Description
The Pet Daily Food Calculator is a specialized tool designed to help pet owners maintain their dog's optimal health through precise nutrition. By calculating the Resting Energy Requirement (RER) and Daily Energy Requirement (DER), this MCP server provides actionable feeding plans. Use `estimate_daily_kcal_requirement` to find your pet's caloric needs, `calculate_daily_gram_intake` to convert those calories into grams based on your specific food's energy density, and `generate_meal_schedule` to determine the ideal number of meals per day. This ensures your dog receives the right amount of nutrients at the correct frequency, whether they are a growing puppy or a senior dog.


## Available Tools
- **estimate_daily_kcal_requirement**: Estimate the daily kilocalorie requirement for a pet
- **generate_meal_schedule**: Generate a daily feeding schedule
- **calculate_daily_gram_intake**: Calculate the daily mass of food in grams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Daily Food Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories does my 5kg puppy need daily?"

**🤖 AI Agent:**
> A 5kg puppy typically requires approximately 280 kcal per day, depending on their activity level.

---

**👤 You:**
> "Calculate the daily food amount for a 20kg adult dog with medium activity using food that has 3.5 kcal/g."

**🤖 AI Agent:**
> For a 20kg adult dog, the daily requirement is approximately 640 kcal, which translates to about 183 grams of food per day.

---

**👤 You:**
> "What is the feeding schedule for a 10kg senior dog?"

**🤖 AI Agent:**
> For a 10kg senior dog, it is recommended to feed 1 to 2 meals per day to maintain stable energy levels.


## Installation & Usage

To install and use the **Pet Daily Food Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-daily-food-calculator](https://vinkius.com/mcp/pet-daily-food-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
