# Baker Percentage Calculator MCP Server

Convert baking recipes between absolute weights (grams) and professional Baker's percentages instantly, making scaling and comparison straightforward.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/baker-percentage-calculator)

## Overview
**Category:** baking
**Tools Count:** 3

## Description
# Professional Recipe Standardization Tool

**Hook:** Have you ever struggled to compare a recipe from a European source (which uses Baker's percentages) with one from an American source (which uses absolute weights)? Or perhaps you need to scale a batch up or down while maintaining perfect proportions?

**Problem:** Baking recipes are highly specialized. Standard units of measure and percentage calculations make cross-regional comparison and professional scaling difficult. Simply measuring ingredients isn't enough; you need to understand the proportional relationship between components.

**Mechanism:** This tool provides three dedicated functions to manage this complexity:
1. **`recipe_to_baker_percentage`**: Takes your raw ingredient weights (e.g., 50g salt, 300g water) and calculates what their professional percentage is relative to the flour base.
2. **`scale_baker_percentage_to_weights`**: If you know a recipe's percentages but need to double or halve the batch size, this function accurately converts those ratios back into precise gram weights based on your scaling factor.
3. **`check_flour_base`**: This is an inverse solver. If you only measure one ingredient (like yeast) and know its percentage (e.g., 1%), this tool calculates the necessary total flour weight to make that measurement accurate.

The system uses these tools to maintain rigorous adherence to established baking standards, ensuring proportional accuracy every time.

**Advantage:** Stop guessing with recipes. Use this connector to transform any set of ingredient weights into standardized professional proportions or scale them precisely for commercial use.


## Available Tools
- **check_flour_base**: Calculate the flour base weight from a known ingredient weight and its Baker's percentage
- **recipe_to_baker_percentage**: Convert ingredient weights to Baker's percentages relative to flour weight
- **scale_baker_percentage_to_weights**: Scale Baker's percentages to absolute weights using a scaling factor


## Installation & Usage

To install and use the **Baker Percentage Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baker-percentage-calculator](https://vinkius.com/mcp/baker-percentage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
