# YMovE Fitness MCP Server

Turn your AI agent into a personal trainer and nutritionist with the YMovE Fitness API. Generate workouts, programs, and meal plans.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ymove-fitness)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Empower your AI agent with professional-grade fitness and nutrition intelligence through **YMovE Fitness**. Access comprehensive databases of exercises, foods, and recipes, or automatically generate customized workout routines and meal plans.

### What you can do

- **Workout Generation** — Instantly create single-session workouts customized by muscle group, equipment, and difficulty
- **Training Programs** — Generate multi-week fitness programs tailored to specific goals like hypertrophy or weight loss
- **Exercise Dictionary** — Access detailed instructions, target muscles, and temporary video demonstrations for hundreds of exercises
- **Meal Plan Generation** — Mathematically generate a full day of meals that hit your exact calorie and macro targets
- **Food Database** — Lookup up nutritional data for generic or branded foods by keyword or barcode (UPC/EAN)
- **Recipe Search** — Find specific recipes filtered by diet constraints (e.g. keto, vegan) and calorie limits

### How it works

1. Subscribe to this server
2. Enter your API Key from the [YMovE Dashboard](https://ymove.app/developer)
3. Start generating workouts and meal plans directly from Claude, Cursor, or your preferred MCP client

When generating exercises, note that video and thumbnail URLs are temporary pre-signed links that expire in 48 hours for security.

### Who is this for?

- **Fitness Enthusiasts** — Log your workouts, discover new exercises, and generate meal plans right in your chat window
- **Personal Trainers** — Rapidly prototype and generate baseline training programs and diets for clients
- **Health App Developers** — Query a centralized database of fitness data without maintaining your own schema


## Available Tools
- **generate_meal_plan**: Generate a daily meal plan reaching a specific calorie target
- **generate_program**: g. "hypertrophy", "weight_loss", "strength").

Generate a multi-week training program
- **generate_workout**: Use this when the user wants a routine for today.

Generate a custom single-session workout
- **get_exercise_details**: Get complete details and instructions for a specific exercise
- **get_food_by_barcode**: Look up a specific food product by its UPC/EAN barcode
- **get_food_details**: Get detailed nutritional breakdown for a specific food
- **get_recipe_details**: Get full recipe details including ingredients and instructions
- **list_exercise_types**: List all valid exercise types (e.g. strength, cardio, stretching)
- **list_muscle_groups**: List all available muscle groups
- **search_exercises**: It returns a list of matching exercises with their IDs, which you need for get_exercise_details.

Search for specific exercises in the YMovE database
- **search_foods**: Search the food database for nutritional values
- **search_recipes**: g. vegan, keto), or maximum calories.

Search for recipes based on diet or calories


## Installation & Usage

To install and use the **YMovE Fitness** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ymove-fitness](https://vinkius.com/mcp/ymove-fitness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
