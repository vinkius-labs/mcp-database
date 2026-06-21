# Training Pace Calculator MCP Server

Calculate running training intensity zones and race pace predictions based on performance or VO2max.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/training-pace-calculator)

## Overview
**Category:** productivity
**Tools Count:** 3

## Description
The Training Pace Calculator MCP server provides precise tools for runners to determine their optimal training intensities. By using `calculate_zones_from_pace`, you can derive specific zones (Easy, Aerobic, Tempo, Interval, and VO2max) in both metric (min/km) and imperial (min/mile) formats based on a recent race result. Alternatively, if you only know your physiological capacity, `calculate_zones_from_vo2max` uses your VO2max value to estimate these same training zones. For runners looking to plan for future goals, the `estimate_distance_conversion` tool utilizes Riegel's formula to predict how your pace might change as you move from shorter distances like a 5K to longer ones like a Marathon.


## Available Tools
- **estimate_distance_conversion**: Uses Riegel's formula.

Predict pace for a different distance based on current performance
- **calculate_zones_from_pace**: g., 5K, 10K). Returns training zones in km and mile formats.

Calculate training intensity zones based on a recent race pace
- **calculate_zones_from_vo2max**: Returns training zones in km and mile formats.

Calculate training intensity zones based on VO2max


## Installation & Usage

To install and use the **Training Pace Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/training-pace-calculator](https://vinkius.com/mcp/training-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
