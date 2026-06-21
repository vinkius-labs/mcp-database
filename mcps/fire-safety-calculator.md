# Fire Safety Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fire-safety-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fire-safety-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fire-safety-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [structural-design](../categories/structural-design.md)

Calculate mandatory fire safety infrastructure requirements, including maximum evacuation distance, minimum stair width, and extinguisher density based on local building codes.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fire Safety Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The new office building has an area of 1500 sqm, a population load of 450 people, and is classified as 'Class B Office'. Check if the evacuation paths are compliant."

**🤖 AI Agent:**
> I will use `calculate_max_walking_distance` with (1500, 450, 'Class B Office'). The result confirms compliance, and the maximum allowed distance is 75 meters. No potential violations found.

---

**👤 You:**
> "We need to know the minimum stair width for a floor with 800 people, using a standard module of 60cm."

**🤖 AI Agent:**
> Running `determine_min_stair_width` with (800, 60) shows the minimum required width is 480 cm. The recommendation suggests using a 528 cm stair for enhanced safety.

---

**👤 You:**
> "For a warehouse space of 900 sqm with 'Medium Risk' classification, how many fire extinguishers are needed?"

**🤖 AI Agent:**
> I executed `specify_extinguisher_requirement` using (900, 'Medium Risk'). The total required is 12 extinguishers: 6 ABC Dry Chemical and 6 Type B Foam.


## Installation & Usage

To install and use the **Fire Safety Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fire-safety-calculator](https://vinkius.com/mcp/fire-safety-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
