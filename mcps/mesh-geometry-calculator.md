# Mesh Geometry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mesh-geometry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Perform advanced geometric and topological analysis on 3D triangle meshes.

## Description
This MCP server provides specialized tools for analyzing the properties of 3D triangular meshes. Using `get_mesh_metrics`, you can calculate surface area, volume, and the center of mass. The `get_mesh_enclosures` tool computes spatial boundaries including Axis-Aligned Bounding Boxes (AABB) and bounding spheres via Ritter's algorithm. For connectivity analysis, use `get_mesh_topology` to detect manifold geometry and compute area-weighted vertex normals.


## Available Tools (3)
- **get_mesh_enclosures**: Calculate AABB and bounding sphere for a mesh
- **get_mesh_metrics**: Calculate surface area, volume, and center of mass for a mesh
- **get_mesh_topology**: Analyze mesh connectivity and surface orientation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mesh Geometry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the surface area and volume of this mesh? Vertices: [0,0,0, 1,0,0, 0,1,0, 0,0,1], Indices: [0,1,2, 0,1,3]"

**🤖 AI Agent:**
> The surface area is 2.0 and the volume is 0.1667.

---

**👤 You:**
> "Calculate the bounding box for these vertices: [0,0,0, 5,5,5]"

**🤖 AI Agent:**
> The AABB min is (0, 0, 0) and max is (5, 5, 5).

---

**👤 You:**
> "Is this mesh manifold? Vertices: [0,0,0, 1,0,0, 0,1,0, 1,1,0], Indices: [0,1,2, 1,2,3]"

**🤖 AI Agent:**
> The mesh is not manifold because some edges are only used by one face.


## ❓ FAQ

**Q: What kind of mesh data should I provide?**
You should provide vertices as a flattened JSON array of numbers (x, y, z coordinates) and indices as a JSON array of integers representing triangle triplets.

**Q: How is the volume calculated?**
The volume is calculated using the signed tetrahedron method relative to the origin. Note that for physically meaningful results, the mesh should be closed (watertight).

**Q: Can I check if my mesh is manifold?**
Yes, the `get_mesh_topology` tool includes a check to determine if every edge in your mesh is shared by exactly two faces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mesh-geometry-calculator](https://vinkius.com/mcp/mesh-geometry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mesh Geometry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mesh-geometry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mesh Geometry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mesh-geometry-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
