# Raw Diet Ratio Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/raw-diet-ratio-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/raw-diet-ratio-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/raw-diet-ratio-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise daily food weights for BARF and PMR raw diets based on pet weight and activity level.

## Description
The Raw Diet Ratio Calculator is a specialized tool for pet owners following biologically appropriate raw feeding protocols like BARF or PMR. By providing your pet's weight and activity level, you can use tools like `calculate_daily_mass_requirement` to find the total daily food mass needed. The server then allows you to use `calculate_component_grams` to partition that mass into exact grams of muscle meat, meaty bones, organs, and vegetables according to the 80/10/5/5 ratio. It ensures your pet receives the correct nutritional balance without guesswork.


## Available Tools
- **calculate_component_grams**: Split total food mass into specific gram amounts for each dietary group
- **calculate_daily_mass_requirement**: Determine the total amount of protein (in grams) needed for a 24-hour period
- **get_protocol_description**: Provide a human-readable explanation of the dietary ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Raw Diet Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much food does my 10kg active dog need daily?"

**🤖 AI Agent:**
> Your 10kg active dog needs a total of 1200 grams of food per day.

---

**👤 You:**
> "Break down the components for 1000g of daily food mass."

**🤖 AI Agent:**
> For 1000g, you need 800g muscle meat, 100g meaty bones, 50g organs, and 50g vegetables.

---

**👤 You:**
> "What does the 80/10/5/5 protocol mean?"

**🤖 AI Agent:**
> The 80/10/5/5 protocol is a nutritional balance of 80% muscle meat, 10% bone, 5% organ, and 5% vegetable.


## Installation & Usage

To install and use the **Raw Diet Ratio Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/raw-diet-ratio-calculator](https://vinkius.com/mcp/raw-diet-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
