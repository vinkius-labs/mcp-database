# Natural Light Estimator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/natural-light-estimator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/natural-light-estimator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/natural-light-estimator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Calculate minimum required window dimensions for natural light and ventilation, ensuring compliance with international building standards.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Natural Light Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a specification report for a house with three rooms: Living Room (50 sqm), Kitchen (25 sqm), and Master Bedroom (30 sqm)."

**🤖 AI Agent:**
> The system will first call `generateRoomSpecificationReport`, which internally uses `calculateRoomMinimums` to find the minimum areas, then determines specific dimensions using `normalizeAreaToWindowDimensions` for all rooms and openings. The final report provides actionable measurements.

---

**👤 You:**
> "I have a 40 sqm living room and want to know the natural light level if I use a 3m x 1.5m window."

**🤖 AI Agent:**
> The system will first run `estimate_light_level` with the specified dimensions (Window Area: 4.5 sqm, Room Area: 40 sqm) and latitude to give a lux estimate. Then, you can use `classify_lighting` on that result for immediate feedback.

---

**👤 You:**
> "What improvements should I make to a room where the light level is classified as 'dim'?"

**🤖 AI Agent:**
> You can use the `recommend_improvements` tool, passing in 'dim' as the category. This will return concrete suggestions for increasing natural light or improving window placement.


## Installation & Usage

To install and use the **Natural Light Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/natural-light-estimator](https://vinkius.com/mcp/natural-light-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
