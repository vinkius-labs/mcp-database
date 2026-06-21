# Bread Proofing Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bread-proofing-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bread-proofing-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bread-proofing-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict fermentation durations for bulk and final proofing based on yeast concentration and temperature.

## Description
This MCP server provides precise estimation tools for bakers to manage fermentation schedules. Using `get_bulk_fermentation_duration`, you can predict the first rise time based on yeast percentage and ambient heat. The `get_final_proof_duration` tool estimates the second rise after shaping. For cold-retarding techniques, `calculate_cold_delay` determines the extra time needed when moving dough to a refrigerator. Finally, use `validate_fermentation_environment` to check if your yeast and temperature settings are within optimal baking parameters.


## Available Tools
- **get_bulk_fermentation_duration**: Estimates the time required for bulk fermentation
- **calculate_cold_delay**: Calculates the additional time required when moving dough to a refrigerator
- **get_final_proof_duration**: Estimates the time required for final proofing
- **validate_fermentation_environment**: Checks if the provided yeast and temperature settings are within safe or standard baking parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bread Proofing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate bulk fermentation for 2% yeast at 25°C."

**🤖 AI Agent:**
> The estimated duration for bulk fermentation is approximately 120 minutes with a high confidence score.

---

**👤 You:**
> "How much extra time is needed if I move dough from 25°C to a 4°C fridge?"

**🤖 AI Agent:**
> Based on the temperature drop, you will need an additional delay of approximately 180 minutes.

---

**👤 You:**
> "Check if 5% yeast at 35°C is a good environment."

**🤖 AI Agent:**
> The environment is viable, but there is a risk of over-proofing due to the high temperature.


## Installation & Usage

To install and use the **Bread Proofing Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bread-proofing-calculator](https://vinkius.com/mcp/bread-proofing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
