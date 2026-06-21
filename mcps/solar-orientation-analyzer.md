# Solar Orientation Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/solar-orientation-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/solar-orientation-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/solar-orientation-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Calculate solar incidence angles, sunlight duration, and architectural protection strategies based on building orientation and latitude.

## Description
The Solar Orientation Analyzer provides specialized tools for architects and engineers to assess solar exposure. Use `calculate_solar_incidence` to determine the sun's angle relative to a facade during summer, winter, and equinox periods. Use `estimate_sunlight_duration` to calculate how many hours of direct sunlight each face receives throughout the year. Finally, use `generate_protection_srategy` to receive architectural recommendations like brise-soleil or reflective glazing based on calculated heat gain risks.


## Available Tools
- **generate_protection_strategy**: Returns recommendation and impact level.

Provides architectural recommendations for solar shading or heat mitigation based on calculated exposure
- **calculate_solar_incidence**: Returns angles for summer, winter, and equinox.

Determines the estimated angle of the sun relative to a specified building facade during different seasonal periods
- **estimate_sunlight_duration**: Returns duration in hours for summer, winter, and equinox.

Estimates how many hours of direct, unshaded sunlight a specific facade receives during different seasons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Orientation Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the solar incidence for a North facing facade in Brasilia?"

**🤖 AI Agent:**
> The `calculate_solar_incidence` tool would provide the specific angles for summer, winter, and equinox based on Brasilia's latitude.

---

**👤 You:**
> "How many hours of sun does an East facing facade get in Sao Paulo?"

**🤖 AI Agent:**
> Using `estimate_sunlight_duration`, you can find the estimated hours of direct sunlight for that orientation during different seasons.

---

**👤 You:**
> "Suggest a protection strategy for a West facing facade in Fortaleza."

**🤖 AI Agent:**
> The `generate_protection_strategy` tool will evaluate the high solar exposure and recommend appropriate architectural interventions.


## Installation & Usage

To install and use the **Solar Orientation Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/solar-orientation-analyzer](https://vinkius.com/mcp/solar-orientation-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
