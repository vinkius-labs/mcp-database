# Fire Safety Calculator MCP Server

Calculate mandatory fire safety infrastructure requirements, including maximum evacuation distance, minimum stair width, and extinguisher density based on local building codes.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fire-safety-calculator)

## Overview
**Category:** structural-design
**Tools Count:** 3

## Description
**The Challenge of Life Safety Compliance**

A commercial or public structure's safety relies entirely on its ability to manage emergencies. Failing to meet fire code standards can result in catastrophic loss of life and property, making compliance a critical structural risk.

**How This System Works**
This MCP connector provides specialized tools that model regulatory requirements based on real-world building physics and local mandates. It connects AI agents directly to the calculation logic needed for safe design.

1. **Evacuation Path Compliance:** Use `calculate_max_walking_distance` with the total area, population load, and construction type to ensure all exit paths are within regulatory limits.
2. **Stairway Capacity:** Utilize `determine_min_stair_width` by feeding it the floor population count and standardized module size (e.g., 60cm) to determine the absolute minimum required stair width.
3. **Fire Suppression Density:** Specify extinguisher needs using `specify_extinguisher_requirement`. Provide the total usable area and the risk class code (A, B, or C) to get an accurate count and distribution of fire suppression equipment.

The resulting data provides a definitive compliance report, ensuring your design meets stringent US and local Brazilian Fire Department standards.


## Available Tools
- **specify_extinguisher_requirement**: Returns distribution by type (A, B, C) and compliance notes for placement.

Determine required fire extinguisher quantity and type distribution by area and risk class
- **determine_min_stair_width**: Returns minimum required width, population ratio details, and safe design recommendation with safety buffer.

Calculate minimum stair width based on population load and module definition
- **calculate_max_walking_distance**: Returns compliance status and violation details.

Calculate maximum walking distance compliance for evacuation paths


## Installation & Usage

To install and use the **Fire Safety Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fire-safety-calculator](https://vinkius.com/mcp/fire-safety-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
