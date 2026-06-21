# Pan Size Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pan-size-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pan-size-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pan-size-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate baking pan volumes and find perfect shape or size substitutions.

## Description
The Pan Size Converter MCP server provides AI agents with precise tools to manage baking consistency. By using `calculate_volume`, agents can determine the exact capacity of any pan shape. The `find_equivalent_pan` tool allows for intelligent substitutions, suggesting alternative pans that maintain the same volume within a specified tolerance. Additionally, `validate_dimensions` ensures all input measurements are physically plausible and compatible with the chosen geometry.


## Available Tools
- **calculate_volume**: Calculates the total volumetric capacity of a specific pan
- **find_equivalent_pan**: Identifies alternative pan shapes and sizes with near-identical volume
- **validate_dimensions**: Verifies that a set of pan dimensions is physically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pan Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the volume of a 22cm round pan with 5cm depth?"

**🤖 AI Agent:**
> The calculated volume for a round pan with a 22cm diameter and 5cm depth is approximately 1900.66 cm³.

---

**👤 You:**
> "Find an alternative for a square pan that is 20cm by 5cm."

**🤖 AI Agent:**
> A suitable alternative found via `find_equivalent_pan` is a round pan with a diameter of approximately 17.8cm and 5cm depth.

---

**👤 You:**
> "Check if these dimensions are valid for a rectangular pan: [20, 10, 5]."

**🤖 AI Agent:**
> The `validate_dimensions` tool confirms that the dimensions [20, 10, 5] are valid for a rectangular pan.


## Installation & Usage

To install and use the **Pan Size Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pan-size-converter](https://vinkius.com/mcp/pan-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
