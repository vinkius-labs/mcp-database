# Natural Light Estimator MCP Server

Calculate minimum required window dimensions for natural light and ventilation, ensuring compliance with international building standards.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/natural-light-estimator)

## Overview
**Category:** architecture
**Tools Count:** 3

## Description
**The Challenge of Passive Design**

Designing a habitable space requires more than just square footage; it demands sufficient natural light and cross-ventilation. Current building codes (like NBR 15575) mandate specific area ratios for openings, but translating these abstract minimums into physically buildable window dimensions is difficult.

**How This System Works**

The Natural Light Estimator addresses this gap by providing a structured workflow that connects code requirements to actionable architectural specifications. It uses specialized tools:

1.  `estimate_light_level`: Calculates the theoretical lux level based on input window and room areas, helping assess immediate light impact.
2.  `normalizeAreaToWindowDimensions`: This core tool takes a required minimum area (e.g., 1/6 of floor space) and calculates optimal width and height dimensions that are structurally plausible for US/EU markets.
3.  `classify_lighting`: Provides context by classifying the resulting lux level into categories like 'adequate' or 'dim', helping pinpoint specific areas needing attention.

**The Advantage**

The system synthesizes these calculations using `generateRoomSpecificationReport` to produce a single, comprehensive report. This report gives architects and builders not just theoretical minimums, but concrete, dimensioned window specifications that meet code while remaining physically feasible for construction.


## Available Tools
- **classify_lighting**: Classify a lux level into dark, dim, adequate, or bright category
- **estimate_light_level**: Estimate natural light level in a room based on window area, room area, and latitude
- **recommend_improvements**: Recommend improvements for a given lighting category


## Installation & Usage

To install and use the **Natural Light Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/natural-light-estimator](https://vinkius.com/mcp/natural-light-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
