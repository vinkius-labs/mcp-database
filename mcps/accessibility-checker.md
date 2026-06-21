# Accessibility Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accessibility-checker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/accessibility-checker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/accessibility-checker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Verify building compliance against universal accessibility standards (USA/EU) for corridors, ramps, and restrooms.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze Room 302. The corridor ID is 'P-MAIN', the measured width is 1.05m, and I need to check ramp compliance for a drop of 1.8m over a horizontal run of 15m with landings."

**🤖 AI Agent:**
> Running checks: `check_corridor_and_passage` confirms passage 'P-MAIN' is compliant (1.05m). `check_ramp_compliance` determines the slope and verifies landing requirements are met.

---

**👤 You:**
> "I need to check a restroom, Room ID 'B-401'. The usable floor area is 2.5 sq meters, and I have installed grab bars."

**🤖 AI Agent:**
> Using `check_bathroom_spaciousness` on Room 'B-401', the tool confirms the area is adequate (2.5m²), and verifies that safety grab bars are in place, ensuring functional compliance.

---

**👤 You:**
> "Check a doorway at 'Lecture Hall Entrance'. The clear opening is 0.9m, and it's a sliding door."

**🤖 AI Agent:**
> The `check_doorway` tool analyzed the location. With an unobstructed width of 0.9m for the 'Lecture Hall Entrance', compliance is confirmed, meeting minimum accessibility standards.


## Installation & Usage

To install and use the **Accessibility Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accessibility-checker](https://vinkius.com/mcp/accessibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
