# API Ninjas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-ninjas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/api-ninjas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/api-ninjas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access fitness, health and nutrition tools — search exercises, calculate calories, body fat, BMR, TDEE and get nutrition info.

## Description
Connect to **API Ninjas** and access a comprehensive suite of health and fitness tools through natural conversation.

### What you can do

- **Exercise Search** — Search 1000+ exercises by name, type, muscle group and difficulty with step-by-step instructions
- **Calories Burned** — Calculate calories burned for various activities based on weight and duration
- **Body Fat** — Estimate body fat percentage using the US Navy method
- **BMR & TDEE** — Calculate Basal Metabolic Rate and Total Daily Energy Expenditure
- **Nutrition** — Get nutritional info for any food item (calories, protein, carbs, fat)
- **Sleep** — Get recommended sleep duration based on age and gender
- **Steps** — Calculate calories burned and distance from step count

### How it works

1. Subscribe to this server
2. Enter your API Ninjas API Key (free registration)
3. Start exploring health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fitness Enthusiasts** — discover exercises, track calories and calculate fitness metrics
- **Personal Trainers** — find exercises by muscle group, calculate client BMR and TDEE
- **Nutritionists** — look up nutritional info for food items and estimate body fat


## Available Tools
- **get_bmr**: Requires weight (kg), height (cm), age and gender. Returns BMR value in calories/day.

Calculate Basal Metabolic Rate
- **get_body_fat**: Requires waist, neck and height measurements (in cm). For women, also requires hip measurement. Returns body fat percentage and category (lean, fitness, acceptable, obese).

Estimate body fat percentage
- **get_calories_burned**: Requires activity name, weight (kg) and duration (minutes). Returns activity name, duration, calories burned and MET value.

Calculate calories burned for an activity
- **get_exercises**: Supports filtering by name, type (cardio, olympic_weightlifting, plyometrics, powerlifting, strength, stretching, strongman), muscle (abdominals, abductors, adductors, biceps, calves, chest, forearms, glutes, hamstrings, lats, lower_back, middle_back, neck, quadriceps, traps, triceps) and difficulty (beginner, intermediate, expert). Returns exercise name, type, muscle worked, equipment needed, difficulty level and step-by-step instructions.

Search exercises by name, type, muscle or difficulty
- **get_nutrition**: Returns calories, protein, carbohydrates, fat, saturated fat, cholesterol, sodium, potassium, fiber and sugar per 100g serving.

Get nutrition info for a food item
- **get_sleep**: Returns recommended sleep range and whether current sleep is adequate.

Get recommended sleep duration
- **get_steps**: Requires step count and optionally weight (kg), height (cm), age and gender for more accurate calculations.

Calculate calories and distance from steps
- **get_tdee**: Requires weight (kg), height (cm), age, gender and activity level. Returns TDEE value in calories/day with breakdown by activity level.

Calculate Total Daily Energy Expenditure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API Ninjas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find chest exercises for beginners."

**🤖 AI Agent:**
> Found 15+ chest exercises for beginners including: Bench Press (barbell, intermediate), Push-ups (body weight, beginner), Cable Crossover (cable, beginner), Dumbbell Fly (dumbbell, beginner). Each with step-by-step instructions.

---

**👤 You:**
> "What's the nutritional info for a banana?"

**🤖 AI Agent:**
> Banana (per 100g): Calories: 89, Protein: 1.1g, Carbs: 22.8g, Fat: 0.3g, Fiber: 2.6g, Sugar: 12.2g, Potassium: 358mg.

---

**👤 You:**
> "Calculate my BMR. I'm 30 years old, male, 80kg, 180cm."

**🤖 AI Agent:**
> Your BMR is 1,795 calories/day. This is the number of calories your body burns at rest. For daily calorie needs, multiply by activity factor (1.2-1.9).


## Installation & Usage

To install and use the **API Ninjas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-ninjas](https://vinkius.com/mcp/api-ninjas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
