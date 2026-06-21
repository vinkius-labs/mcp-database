# Geometry Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geometry-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/geometry-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/geometry-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Compute exact Euclidean distances, 2D areas, and 3D volumes completely local. A zero-latency geometry engine for autonomous AI agents.

## Description
Spatial reasoning and geometric calculations are frequent stumbling blocks for Large Language Models. The Geometry Calculator MCP Server provides your AI with a deterministic engine to solve complex spatial problems instantly.

### The Superpowers
- **Exact Dimensions:** Flawlessly calculate 2D areas (circles, rectangles, triangles) and 3D volumes (spheres, cubes, cylinders, prisms).
- **Spatial Distances:** Compute exact Euclidean distances across 2D planes or 3D Cartesian space instantly.
- **Absolute Privacy (Local):** Never send sensitive architectural or engineering coordinates over the internet. Calculations happen 100% locally.
- **Zero Hallucination:** Replaces LLM probabilistic guessing with absolute mathematical certainty.


## Available Tools
- **calculate_2d_area**: For circle: {"radius": x}. For rectangle: {"width": x, "height": y}. For triangle: {"base": x, "height": y}.

Calculates the exact area of 2D shapes (circle, rectangle, triangle)
- **calculate_distance**: 2D example: {"x": 0, "y": 0}. 3D example: {"x": 1, "y": 2, "z": 3}.

Calculates the Euclidean distance between two points in 2D or 3D space
- **calculate_3d_volume**: Sphere: {"radius": x}. Cube: {"side": x}. Cylinder: {"radius": x, "height": y}. Prism: {"width": x, "height": y, "depth": z}.

Calculates the exact volume of 3D shapes (sphere, cube, cylinder, prism)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geometry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the area of a circle with a radius of 7.5 units."

**🤖 AI Agent:**
> Using the calculate_2d_area tool (shape='circle', params={"radius": 7.5}): The exact area is 176.71458.

---

**👤 You:**
> "What is the volume of a cylinder with radius 5 and height 10?"

**🤖 AI Agent:**
> Using the calculate_3d_volume tool (shape='cylinder', params={"radius": 5, "height": 10}): The volume is 785.398.

---

**👤 You:**
> "Calculate the Euclidean distance between point A (0, 0, 0) and point B (3, 4, 12)."

**🤖 AI Agent:**
> Using the calculate_distance tool: The exact Euclidean distance is 13.


## Installation & Usage

To install and use the **Geometry Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geometry-calculator](https://vinkius.com/mcp/geometry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
