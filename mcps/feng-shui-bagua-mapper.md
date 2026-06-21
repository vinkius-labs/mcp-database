# Feng Shui Bagua Mapper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feng-shui-bagua-mapper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feng-shui-bagua-mapper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feng-shui-bagua-mapper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Aligns a Bagua map to your floor plan based on entrance orientation.

## Description
The Feng Shui Bagua Mapper connects your physical space to the ancient Bagua energy map. By providing the orientation of your main entrance, you can use `orientationTool` to calculate the rotation, then apply `mapAreaTool` or `analyzeLayoutTool` to identify which life areas--such as Wealth, Love, or Career--correspond to each room in your home. This tool bridges the gap between architectural layouts and spatial energy analysis.


## Available Tools
- **get_orientation_offset**: Converts various entrance descriptions into a standardized numerical rotation value
- **analyze_room_layout**: Takes a collection of rooms and produces a complete mapping of room names to their corresponding Life Areas
- **map_coordinate_to_area**: Determines which single Life Area covers a specific point in space given a rotation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feng Shui Bagua Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the rotation offset for a North entrance?"

**🤖 AI Agent:**
> A North entrance corresponds to a 0 degree rotation offset.

---

**👤 You:**
> "Analyze this room: Name: Kitchen, X: 5, Y: -2 with a 45 degree offset."

**🤖 AI Agent:**
> The Kitchen is located in the Wealth & Prosperity sector.

---

**👤 You:**
> "Map a layout with two rooms: Living Room (0, 0) and Bedroom (2, 2), rotation offset 90."

**🤖 AI Agent:**
> The Living Room maps to the Career & Life Path area, and the Bedroom maps to the Children & Creativity area.


## Installation & Usage

To install and use the **Feng Shui Bagua Mapper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feng-shui-bagua-mapper](https://vinkius.com/mcp/feng-shui-bagua-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
