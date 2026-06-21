# Thermal Mass Estimator MCP Server

Calculate thermal lag, amplitude damping, and U-value for wall structures based on material properties.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/thermal-mass-estimator)

## Overview
**Category:** construction
**Tools Count:** 3

## Description
This MCP server provides specialized tools to quantify the thermal performance of building envelopes. Use `get_material_properties` to retrieve conductivity, density, and specific heat for materials like brick or concrete. Use `calculate_u_value` to determine thermal transmittance based on wall thickness. You can also use `estimate_thermal_behavior` to project how much temperature fluctuations are reduced (damping) and the time delay (lag) of heat moving through a structure.


## Available Tools
- **calculate_u_value**: Calculates the thermal transmittance (U-value) for a single layer of material
- **estimate_thermal_behavior**: Estimates the thermal lag and amplitude damping factor for a wall layer
- **get_material_properties**: Retrieves the fundamental thermal properties for a specific building material


## Installation & Usage

To install and use the **Thermal Mass Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thermal-mass-estimator](https://vinkius.com/mcp/thermal-mass-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
