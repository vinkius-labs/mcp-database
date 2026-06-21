# Haversine Distance Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/haversine-distance-engine-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/haversine-distance-engine-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/haversine-distance-engine-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate precise geographic distances between GPS coordinates instantly. Uses the Haversine formula for exact spherical routing.

## Description
LLMs lack spatial and geometric reasoning. If an AI agent attempts to calculate the distance between two GPS coordinates, it often returns a hallucinated straight-line guess that ignores the Earth's spherical shape. This MCP solves that by bringing mathematical geometric precision to the edge.

### The Superpowers

- **Haversine Math:** Executes the complex spherical trigonometry formula instantly to calculate the exact distance over the Earth's surface.
- **Multi-Unit Precision:** Native support for Kilometers, Miles, Meters, and Nautical Miles without manual float conversions.


## Available Tools
- **haversine_calculate_distance**: Pass latitude and longitude for both points. The engine uses the Haversine formula to return the distance in kilometers and miles.

Calculates the exact geographic distance between two GPS coordinates using the mathematical Haversine formula


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Haversine Distance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the exact geographic distance in kilometers between London (51.5074, -0.1278) and Paris (48.8566, 2.3522)."

**🤖 AI Agent:**
> ✅ **Calculation Complete:** The exact Haversine distance is `343.46` km.

---

**👤 You:**
> "What is the distance in miles from the warehouse (-23.5505, -46.6333) to the delivery address (-22.9068, -43.1729)?"

**🤖 AI Agent:**
> ✅ **Result:** The spherical distance is `223.32` miles.

---

**👤 You:**
> "Convert the distance between these coordinates into exact meters for a micro-mobility agent."

**🤖 AI Agent:**
> ✅ **Geo Metrics:** The coordinates are exactly `1,250.45` meters apart.


## Installation & Usage

To install and use the **Haversine Distance Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/haversine-distance-engine-alternative](https://vinkius.com/mcp/haversine-distance-engine-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
