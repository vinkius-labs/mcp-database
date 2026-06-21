# Accessibility Checker MCP Server

Verify building compliance against universal accessibility standards (USA/EU) for corridors, ramps, and restrooms.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accessibility-checker)

## Overview
**Category:** construction
**Tools Count:** 4

## Description
**Goal:** Ensure every physical space meets minimum dimensions required for people with reduced mobility.

**Problem:** Building designs often fail to meet modern accessibility standards (like ADA or European norms). A small mistake in a corridor width, ramp slope, or bathroom layout can render an entire facility unusable and dangerous. Failing compliance blocks safe passage for wheelchairs and other aids.

**Mechanism:** This service provides precise checks across all critical architectural elements using specialized tools:
*   `check_corridor_and_passage`: Verifies that hallways maintain a minimum clear width throughout their length.
*   `check_ramp_compliance`: Calculates the slope of ramps and confirms adequate resting landings at every transition point.
*   `check_doorway`: Measures the actual clear opening width to ensure passage is possible for mobility aids.
*   `check_bathroom_spaciousness`: Confirms that restrooms provide enough functional floor area and maneuvering space, going beyond simple dimensions.

**Advantage:** By running these checks, you receive an immediate compliance report detailing every violation--from minor dimension gaps to critical structural failures--allowing architects and builders to correct issues before construction begins.


## Available Tools
- **check_bathroom_spaciousness**: Confirm bathroom provides enough functional space for mobility aid maneuverability
- **check_corridor_and_passage**: Returns compliance status and violation details.

Verify corridor or passage meets minimum clear width for universal access
- **check_doorway**: Verify doorway provides adequate clear opening width for mobility aid users
- **check_ramp_compliance**: 33% maximum standard and checks for required transition landings.

Determine if a ramp section meets maximum slope and landing requirements


## Installation & Usage

To install and use the **Accessibility Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accessibility-checker](https://vinkius.com/mcp/accessibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
