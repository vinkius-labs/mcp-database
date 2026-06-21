# Pet Calorie Needs MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-calorie-needs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pet-calorie-needs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pet-calorie-needs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Calculate precise daily energy requirements (RER and MER) for pets based on weight and lifestyle.

## Description
This MCP server provides veterinary-standard calculations for a pet's nutritional needs. Using the `calculate_rer` tool, you can determine the Resting Energy Requirement based on metabolic weight. By applying lifestyle multipliers via `calculate_mer`, you can find the Maintenance Energy Requirement (MER) for various states like neutered, intact, or athletic. Use `list_lifestyle_factors` to see all available activity and physiological multipliers.


## Available Tools
- **calculate_mer**: Calculate the Maintenance Energy Requirement (MER) for a pet
- **calculate_rer**: 75 to find the baseline calories needed at rest.

Calculate the Resting Energy Requirement (RER) for a pet
- **list_lifestyle_factors**: List all available lifestyle factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Calorie Needs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories does a 10kg dog need if it is neutered?"

**🤖 AI Agent:**
> A 10kg neutered dog has an RER of approximately 501 kcal and a daily maintenance requirement (MER) of about 626 kcal.

---

**👤 You:**
> "Calculate the RER for a 5kg cat."

**🤖 AI Agent:**
> The Resting Energy Requirement (RER) for a 5kg cat is approximately 297 kcal.

---

**👤 You:**
> "What are the available lifestyle factors?"

**🤖 AI Agent:**
> The available lifestyle factors include neutered, intact, pregnant, lactating, athletic, and weight loss.


## Installation & Usage

To install and use the **Pet Calorie Needs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-calorie-needs](https://vinkius.com/mcp/pet-calorie-needs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
