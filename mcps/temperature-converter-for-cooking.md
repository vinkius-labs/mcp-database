# Temperature Converter for Cooking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/temperature-converter-for-cooking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/temperature-converter-for-cooking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/temperature-converter-for-cooking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert oven temperatures between Celsius, Fahrenheit, and the European Gas scale with heat intensity classification.

## Description
This MCP server provides precise temperature conversions for cooking environments. It allows AI agents to convert between Celsius, Fahrenheit, and the European Gas oven scale (1-9). Beyond simple unit conversion, it also classifies the heat intensity as Low, Medium, High, or Very High based on the resulting temperature. Use tools like `fahrenheit_from_celsius`, `celsius_from_fahrenheit`, and `oven_settings_from_gas` to get accurate cooking instructions.


## Available Tools
- **celsius_from_fahrenheit**: Convert Fahrenheit to Celsius
- **fahrenheit_from_celsius**: Convert Celsius to Fahrenheit
- **oven_settings_from_gas**: Get oven settings from gas knob position


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temperature Converter for Cooking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is 180 degrees Celsius in Fahrenheit?"

**🤖 AI Agent:**
> 180°C is approximately 356°F, which corresponds to a High heat level.

---

**👤 You:**
> "Convert gas setting 4 to Celsius."

**🤖 AI Agent:**
> Gas setting 4 corresponds to approximately 150°C (302°F), which is a Medium heat level.

---

**👤 You:**
> "What temperature is 400 Fahrenheit in Celsius?"

**🤖 AI Agent:**
> 400°F is approximately 204.4°C, which falls under the Very High heat level.


## Installation & Usage

To install and use the **Temperature Converter for Cooking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temperature-converter-for-cooking](https://vinkius.com/mcp/temperature-converter-for-cooking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
