# ExerciseDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exercisedb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/exercisedb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/exercisedb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Access 1300+ exercises with body parts, target muscles, equipment, instructions and animated GIFs.

## Description
Connect to **ExerciseDB** and explore a comprehensive exercise database through natural conversation.

### What you can do

- **Exercise Search** — Browse 1300+ exercises with detailed instructions and animated GIFs
- **Filter by Body Part** — Find exercises for back, chest, shoulders, legs, arms, waist and more
- **Filter by Target Muscle** — Search exercises targeting specific muscles (abs, biceps, quads, glutes)
- **Filter by Equipment** — Find exercises by equipment type (dumbbell, barbell, body weight, cable)
- **Search by Name** — Find exercises by name (crunches, curls, presses, squats)
- **Reference Lists** — Get complete lists of body parts, target muscles and equipment types

### How it works

1. Subscribe to this server
2. Enter your ExerciseDB API Key (from RapidAPI)
3. Start exploring exercises from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fitness Enthusiasts** — discover new exercises, build workout routines and learn proper form
- **Personal Trainers** — find exercises by equipment, body part or target muscle for client programs
- **App Developers** — integrate exercise data with instructions and animations into fitness apps


## Available Tools
- **get_all_exercises**: Returns exercise names, body parts, target muscles, equipment needed, GIF URLs and step-by-step instructions. Supports limit and offset parameters for pagination.

Get all exercises with pagination
- **get_body_part_list**: Useful for discovering valid body part values to use with get_exercises_by_body_part.

Get list of all body parts
- **get_equipment_list**: Useful for discovering valid equipment values to use with get_exercises_by_equipment.

Get list of all equipment types
- **get_exercise_by_id**: Returns exercise name, body part, target muscle, equipment, secondary muscles, step-by-step instructions and animated GIF URL.

Get a specific exercise by ID
- **get_exercises_by_body_part**: Common body parts include: "back", "chest", "shoulders", "upper arms", "lower arms", "upper legs", "lower legs", "neck", "waist", "cardio". Returns exercise details with target muscles, equipment and instructions.

Get exercises by body part
- **get_exercises_by_equipment**: Common equipment includes: "assisted", "band", "barbell", "body weight", "bosu ball", "cable", "dumbbell", "elliptical machine", "ez barbell", "hammer", "kettlebell", "leverage machine", "medicine ball", "olympic barbell", "resistance band", "roller", "rope", "skierg machine", "sled machine", "smith machine", "stability ball", "stationary bike", "stepmill machine", "tire", "trap bar", "upper body ergometer", "weighted", "wheel roller". Returns exercise details with body part, target muscles and instructions.

Get exercises by equipment type
- **get_exercises_by_name**: Returns matching exercises with full details including body part, target muscles, equipment, instructions and GIF URLs.

Get exercises by name search
- **get_exercises_by_target**: Common targets include: "abductors", "abs", "adductors", "biceps", "calves", "cardiovascular system", "delts", "forearms", "glutes", "hamstrings", "lats", "levator scapulae", "pectorals", "quads", "serratus anterior", "spine", "traps", "triceps", "upper back". Returns exercise details with body part, equipment and instructions.

Get exercises by target muscle
- **get_target_list**: Useful for discovering valid target values to use with get_exercises_by_target.

Get list of all target muscles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ExerciseDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me exercises for chest with dumbbells."

**🤖 AI Agent:**
> Found 15+ chest exercises with dumbbells including: Dumbbell Bench Press, Dumbbell Fly, Incline Dumbbell Press, Decline Dumbbell Fly. Each includes step-by-step instructions and animated GIF.

---

**👤 You:**
> "What exercises target the abs?"

**🤖 AI Agent:**
> Found 50+ exercises targeting abs including: Crunches, Plank, Bicycle Crunches, Russian Twist, Leg Raises, Mountain Climbers. Each with instructions, body part, equipment needed and GIF.

---

**👤 You:**
> "Show me exercises I can do with just body weight."

**🤖 AI Agent:**
> Found 100+ body weight exercises including: Push-ups, Pull-ups, Squats, Lunges, Plank, Burpees, Dips. No equipment needed — perfect for home workouts.


## Installation & Usage

To install and use the **ExerciseDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exercisedb](https://vinkius.com/mcp/exercisedb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
