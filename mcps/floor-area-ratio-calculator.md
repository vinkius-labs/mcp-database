# Floor Area Ratio Calculator MCP Server

Calculate maximum buildable footprint, total floor area, and green space compliance for any plot size in seconds.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/floor-area-ratio-calculator)

## Overview
**Category:** real-estate
**Tools Count:** 3

## Description
## Building Development Feasibility Analysis

The process of developing a property is complex. It requires coordinating multiple, often conflicting, zoning constraints--from how much ground area you can cover (Site Coverage) to the total bulk allowed over all floors (FAR), and ensuring enough space for water absorption (Permeability).

**The Problem:** Traditional planning assessments are manual, slow, and require an expert to track these three distinct metrics simultaneously. A developer might calculate a high FAR but fail because they neglected minimum permeable area requirements, or vice versa.

**The Mechanism:** This MCP connects your AI agent directly to the core formulas of urban planning law. It uses three specialized functions to assess viability: 

1.  `max_site_coverage`: Determines the maximum *ground footprint* allowed by zoning occupancy limits for a given plot size.
2.  `max_total_area`: Calculates the total permitted floor area (FAR) across all stories, ensuring overall density compliance.
3.  `calculate_permeability`: Verifies that enough open, non-impervious space remains after accounting for building foundations and meeting minimum green space mandates.

By chaining these tools, your agent can perform a complete, multi-faceted feasibility check in one workflow, identifying the most restrictive constraint immediately.

**The Advantage:** You get instant, quantitative compliance checks against complex municipal codes. This moves development planning from guesswork to guaranteed calculation support.


## Available Tools
- **max_site_coverage**: Takes plot area and maximum site coverage percentage as inputs.

Calculate the maximum allowable ground footprint area for building construction based on site coverage limits
- **max_total_area**: Takes plot area, FAR percentage, and optionally a site coverage footprint area.

Calculate the maximum total floor area allowed on a plot based on Floor Area Ratio restrictions
- **calculate_permeability**: Takes lot area, minimum permeability percentage, and optionally a building footprint area.

Calculate minimum permeable area required and available buildable ground after accounting for green space requirements


## Installation & Usage

To install and use the **Floor Area Ratio Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/floor-area-ratio-calculator](https://vinkius.com/mcp/floor-area-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
