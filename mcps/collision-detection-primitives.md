# Collision Detection Primitives MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/collision-detection-primitives)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate 3D intersections, penetrations, and impact timings for spheres, AABBs, rays, and planes.

## Description
This MCP server provides a specialized computational engine for high-precision geometric intersection testing. Use `spherical_collision` to determine if two spheres overlap and find contact details like penetration depth. The `box_collision` tool checks intersections between spheres and axis-aligned bounding boxes (AABB). For ray casting, `ray_intersection` calculates the time of impact and hit points using the slab method for AABBs. Additionally, `boundary_inclusion` verifies if a sphere is contained within specific bounds.


## Available Tools (4)
- **boundary_inclusion**: Check if a sphere is within bounds
- **box_collision**: Check collision between a sphere and an AABB
- **ray_intersection**: Check intersection between a ray and an AABB
- **spherical_collision**: Check intersection between two spheres


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collision Detection Primitives** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are these two spheres colliding? Sphere A: {"center": {"x": 0, "y": 0, "z": 0}, "radius": 5}, Sphere B: {"center": {"x": 8, "y": 0, "z": 0}, "radius": 4}"

**🤖 AI Agent:**
> Yes, the spheres are intersecting. The penetration depth is 1.0 and the contact point is at (5, 0, 0).

---

**👤 You:**
> "Check if this ray hits the box: Ray: {"origin": {"x": -5, "y": 0, "z": 0}, "direction": {"x": 1, "y": 0, "z": 0}}, AABB: {"min": {"x": -1, "y": -1, "z": -1}, "max": {"x": 1, "y": 1, "z": 1}}"

**🤖 AI Agent:**
> The ray intersects the AABB. The time of impact is 4.0 and the hit point is (-1, 0, 0).

---

**👤 You:**
> "Is this sphere inside the bounds? Sphere: {"center": {"x": 0, "y": 0, "z": 0}, "radius": 1}, AABB: {"min": {"x": -2, "y": -2, "z": -2}, "max": {"x": 2, "y": 2, "z": 2}}"

**🤖 AI Agent:**
> Yes, the sphere is entirely within the specified AABB boundaries.


## ❓ FAQ

**Q: What types of primitives are supported?**
The server supports spheres, Axis-Aligned Bounding Boxes (AABB), rays, and planes for various intersection tests.

**Q: How do I use the `spherical_collision` tool?**
Provide two JSON strings representing spheres, each containing a center (x, y, z) and a radius.

**Q: Does the server provide penetration depth?**
Yes, for collision tests like `box_collision`, the tool returns the penetration depth and the contact point.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/collision-detection-primitives](https://vinkius.com/mcp/collision-detection-primitives)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collision Detection Primitives** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `collision-detection-primitives` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collision Detection Primitives** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collision-detection-primitives": {
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
