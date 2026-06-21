# Shading Device Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shading-device-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shading-device-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shading-device-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise dimensions for horizontal and vertical solar shading devices.

## Description
This MCP server provides specialized tools for architectural thermal comfort. Use `get_solar_position` to determine the sun's altitude and azimuth, then use `calculate_horizontal_depth` to find the minimum projection required for horizontal louvers or `calculate_vertical_width` for vertical fins. You can also audit existing structures using `validate_compliance` to ensure they meet your target solar cutoff angles.


## Available Tools
- **calculate_vertical_width**: Calculate minimum width for vertical fins
- **validate_compliance**: Validate shading device compliance
- **calculate_horizontal_depth**: Calculate minimum depth for horizontal louvers
- **get_solar_position**: Calculate the sun position


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shading Device Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the sun's position at latitude 40.7128 on day 150 at 12:00?"

**🤖 AI Agent:**
> By calling `get_solar_position`, the tool will return the specific solar altitude and azimuth for that location and time.

---

**👤 You:**
> "Calculate required depth for a horizontal louver at latitude 40, surface azimuth 180, solar altitude 45, solar azimuth 135, and cutoff angle 60."

**🤖 AI Agent:**
> The `calculate_horizontal_depth` tool will compute the minimum projection depth needed to satisfy the 60-degree cutoff requirement.

---

**👤 You:**
> "Check if a 0.5m depth louver is compliant with a 45 degree target angle."

**🤖 AI Agent:**
> The `validate_compliance` tool will analyze the geometry and return whether the device meets the design threshold or if there is a failure margin.


## Installation & Usage

To install and use the **Shading Device Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shading-device-calculator](https://vinkius.com/mcp/shading-device-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
