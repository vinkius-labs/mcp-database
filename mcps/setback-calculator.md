# Setback Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/setback-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/setback-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/setback-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Determine maximum buildable area and optimal land utilization by applying local zoning setback rules.

## Description
**Need to know how much you can actually build on your lot?** Zoning laws dictate strict minimum setbacks (distances from property lines) that cannot be ignored. Ignoring these rules means building illegally and facing costly revisions.


## Available Tools
- **calculate_building_footprint**: Calculate the total buildable area and perimeter from usable envelope dimensions
- **calculate_land_utilization_metrics**: Percentage is capped at 100% if footprint exceeds total area.

Calculate how efficiently the plot is used by comparing built footprint area against total land area
- **calculate_usable_dimensions**: Returns the maximum allowable building envelope dimensions in meters.

Calculate the actual buildable dimensions after applying mandatory setback requirements to lot measurements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Setback Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a lot that is 40m long and 25m wide. My local code requires a 5m front setback, 3m rear setback, and 4m side setbacks on both sides. What are my buildable dimensions?"

**🤖 AI Agent:**
> To find this, I will execute the `calculate_usable_dimensions` tool with lotLengthMeters=40, lotWidthMeters=25, frontSetbackMeters=5, rearSetbackMeters=3, sideA_setbackMeters=4, and sideB_setbackMeters=4. The result will give me the maximum usable length and width.

---

**👤 You:**
> "Using my restricted dimensions of 32m by 17m, what is the total buildable area and perimeter?"

**🤖 AI Agent:**
> I will run `calculate_building_footprint` with usableLengthMeters=32 and usableWidthMeters=17. This provides the total footprint area in square meters, which is essential for zoning submissions.

---

**👤 You:**
> "If my lot's total area is 800 sq.m., and the building footprint is 512 sq.m., what percentage of land can I actually use?"

**🤖 AI Agent:**
> I will call `calculate_land_utilization_metrics` using totalLandAreaSqMeters=800 and buildingFootprintAreaSqMeters=512. This calculation gives the utilization percentage, confirming compliance.


## Installation & Usage

To install and use the **Setback Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/setback-calculator](https://vinkius.com/mcp/setback-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
