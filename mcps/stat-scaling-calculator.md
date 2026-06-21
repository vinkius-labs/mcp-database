# Stat Scaling Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stat-scaling-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stat-scaling-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stat-scaling-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Compute and compare attribute progression curves for game design.

## Description
This MCP server provides game designers with precise mathematical tools to define how attributes like Strength, Health, or Mana evolve from Level 1 to a maximum level. Using `compute_progression_table`, you can generate detailed level-by-level breakdowns for various growth archetypes including linear, exponential, and S-curves. The `analyze_growth_velocity` tool helps identify unintended power spikes by calculating the delta between levels, while `compare_scaling_strategies` allows for a unified visual comparison of multiple scaling configurations to ensure consistent progression feel.


## Available Tools
- **compare_scaling_strategies**: Produces a unified dataset for visual comparison of different scaling configurations
- **analyze_growth_velocity**: Calculates the incremental change in an attribute's value between consecutive levels
- **compute_progression_table**: Generates a complete step-by-step breakdown of an attribute's value for every level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stat Scaling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a linear progression table from 10 to 100 up to level 50."

**🤖 AI Agent:**
> The `compute_progression_table` tool will generate a breakdown where each level increases by exactly 1.837...

---

**👤 You:**
> "Analyze the growth velocity of this table: [{"level": 1, "statValue": 10}, {"level": 2, "statValue": 15}]"

**🤖 AI Agent:**
> The `analyze_growth_velocity` tool shows a delta of 5 at level 2.

---

**👤 You:**
> "Compare an exponential curve (10 to 500, lvl 20) with a linear curve (10 to 500, lvl 20)."

**🤖 AI Agent:**
> The `compare_scaling_strategies` tool will provide a unified dataset for visual comparison.


## Installation & Usage

To install and use the **Stat Scaling Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stat-scaling-calculator](https://vinkius.com/mcp/stat-scaling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
