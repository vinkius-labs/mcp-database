# Room Proportion Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/room-proportion-checker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/room-proportion-checker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/room-proportion-checker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Checks if a room's dimensions meet ergonomic and architectural standards for visual harmony.

## Description
**Room Proportion Checker**: Does your space feel right? Many rooms fail basic ergonomic or proportional tests, leading to a feeling of discomfort or imbalance. This service evaluates the structural harmony and compliance of any given room volume (Width x Length x Height) against established architectural standards. It calculates multiple indices to determine if the proportions are visually pleasing and functional for human use.


## Available Tools
- **calculate_axis_balance_ratio**: Higher scores mean more harmonious proportions.

Calculate the axis balance ratio for a room based on width, length, and height
- **evaluate_floor_area_index**: If height is omitted, a default of 2.5m is used.

Evaluate the floor area index relating surface area to ceiling height
- **classify_room_proportions**: Classify overall room proportions as well-proportioned or requiring correction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Proportion Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check a living room with 6m width, 10m length, and 2.8m height."

**🤖 AI Agent:**
> The proportions are generally good, but the `calculate_axis_balance_ratio` indicates a slight elongation bias (L > W). The overall grade from `classify_room_proportions` is 'Well Proportioned' with minor suggested corrections.

---

**👤 You:**
> "Analyze a small bathroom: 2m width, 1.5m length, and 2.4m height."

**🤖 AI Agent:**
> The `evaluate_floor_area_index` suggests the surface area is highly suitable for this height. However, the overall result from `classify_room_proportions` recommends correction due to minimum circulation clearance issues.

---

**👤 You:**
> "What are the ideal proportions for a bedroom of 4m by 5m?"

**🤖 AI Agent:**
> Running through `calculate_axis_balance_ratio` and `evaluate_floor_area_index` suggests ideal proportions are close to square. For 4x5m, the current dimensions yield a good FAI score, but increasing the height would improve overall balance.


## Installation & Usage

To install and use the **Room Proportion Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/room-proportion-checker](https://vinkius.com/mcp/room-proportion-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
