# Pet Water Intake Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-water-intake-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pet-water-intake-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pet-water-intake-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate optimal daily water intake for dogs and cats based on weight, food type, and temperature.

## Description
The Pet Water Intake Calculator helps pet owners ensure their animals stay hydrated by calculating precise supplemental water needs. By analyzing species (dog or cat), weight, food moisture content (dry, wet, or raw), and ambient temperature, the server provides actionable hydration targets. Use `calculate_daily_intake` to find specific milliliter requirements, `check_dehydration_indicators` to identify physical warning signs like lethargy or skin elasticity changes, and `get_food_moisture_profile` to understand how different diets impact hydration needs.


## Available Tools
- **calculate_daily_intake**: Calculates the total volume of supplemental water (in ml) a pet needs daily
- **check_dehydration_indicators**: Identifies physical warning signs of dehydration
- **get_food_moisture_profile**: Provides moisture content information for each food type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Water Intake Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much water does my 10kg dog need if I feed him dry food and it is 30 degrees Celsius?"

**🤖 AI Agent:**
> Your 10kg dog needs approximately 250ml of supplemental water daily. The high temperature and dry food increase the requirement.

---

**👤 You:**
> "What are the signs of dehydration for a cat in hot weather?"

**🤖 AI Agent:**
> In high temperatures, you should monitor for lethargy and changes in skin elasticity.

---

**👤 You:**
> "How much moisture is in wet food?"

**🤖 AI Agent:**
> Wet food provides a high percentage of hydration, significantly reducing the need for supplemental drinking water.


## Installation & Usage

To install and use the **Pet Water Intake Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-water-intake-calculator](https://vinkius.com/mcp/pet-water-intake-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
