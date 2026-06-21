# NotCo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notco)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/notco-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/notco-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Interact with Giuseppe AI, NotCo's proprietary plant-based formulation engine, to analyze ingredients, match flavor profiles, and generate recipes.

## Description
Connect your AI agent directly to **Giuseppe**, NotCo’s proprietary Food Tech AI platform. Accelerate your B2B food research and development by commanding Giuseppe through natural language.

### What you can do

- **AI Formulation Generation** — Command Giuseppe to analyze the molecular structure of an animal product and generate a plant-based blueprint using combinations from a database of over 300,000 plants
- **Ingredient Search** — Browse and retrieve the molecular, sensory, and functional profiles of thousands of plant extracts and proteins
- **Flavor & Texture Matching** — Use AI computational models to find plant compounds that replicate specific volatile molecules, aromas, and mouthfeels
- **Nutritional Label Prediction** — Run predictive algorithms on custom plant mixtures to estimate the final nutritional values of a recipe before entering the lab
- **Cost Estimation** — Predict the theoretical mass-production cost of an AI-generated formula based on global commodity pricing

### How it works

1. Subscribe to this server
2. Enter your NotCo API Key (partner access required)
3. Start exploring formulations from Claude, Cursor, or your preferred MCP client

### Who is this for?

- **Food Scientists & R&D Teams** — instantly query molecular matches without switching contexts
- **Product Formulators** — test theoretical plant-based recipes in a virtual environment before lab prototyping
- **Strategic Food Partners** — monitor project progress and evaluate AI-generated prototypes rapidly


## Available Tools
- **analyze_nutrition**: Analyze the nutritional output of a formulation
- **create_formulation**: Request a new AI formulation
- **create_project**: Create a new R&D project
- **estimate_cost**: Predict the mass production cost of a formulation
- **get_formulation**: Get details of a specific AI formulation
- **get_ingredient**: Get complete molecular profile of an ingredient
- **list_formulations**: g., dairy, meat, sauces).

List plant-based AI formulations
- **list_ingredients**: Search the plant-based ingredient molecular database
- **list_nutritional_profiles**: List target nutritional benchmarks
- **list_projects**: List active R&D projects
- **list_sensory_profiles**: List standard sensory profiles
- **list_suppliers**: List approved ingredient suppliers
- **run_sensory_test**: Run an AI simulation of a sensory test
- **search_flavor_matches**: Find plant combinations that mimic a target flavor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NotCo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask Giuseppe to create a plant-based alternative for condensed milk, with the constraint 'no palm oil'."

**🤖 AI Agent:**
> Giuseppe generated Formulation ID #CM-882. The top ingredient matches include: Coconut Oil (35%), Faba Bean Protein isolate (18%), Cabbage Extract (for molecular lactose emulation - 2%), and Beet fiber. The theoretical match score on viscosity and flavor is 92.4%.

---

**👤 You:**
> "Run a nutritional analysis on formulation ID #CM-882."

**🤖 AI Agent:**
> Predictive nutritional analysis for Formulation #CM-882 (per 100g): Calories: 325kcal, Total Fat: 11g (Saturated 8g, Trans 0g), Total Carbohydrate: 55g (Sugars 54g), Protein: 3g. Compared to standard dairy condensed milk, this formulation achieves a 15% reduction in saturated fats while maintaining identical sugar curves.

---

**👤 You:**
> "Estimate the mass-production cost for this formulation."

**🤖 AI Agent:**
> Based on current global commodity rates for the specified plant extracts (Coconut Oil, Faba Bean, etc.), the estimated cost for Formulation #CM-882 is $1.15 USD per kg. This represents a 12% cost advantage compared to the current dairy milk spot pricing.


## Installation & Usage

To install and use the **NotCo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notco](https://vinkius.com/mcp/notco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
