# Field of View & Frustum Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/field-of-view-frustum-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate precise frustum geometry, object visibility, and LOD recommendations for 3D engines.

## Description
This MCP server provides deterministic mathematical tools for 3D game engine optimization. It allows AI agents to calculate precise frustum dimensions, determine if objects are within the camera's view using `test_object_visibility`, and generate optimized Level of Detail (LOD) strategies via `calculate_lod_recommendations`. Use `calculate_frustum_geometry` to derive horizontal FOV and plane dimensions, or `calculate_culling_efficiency` to measure rendering performance by analyzing culled object counts.


## Available Tools (4)
- **calculate_frustum_geometry**: Calculates the fundamental angular and dimensional properties of the camera's view frustum
- **calculate_culling_efficiency**: Provides a metric to evaluate how effectively the engine is skipping non-visible objects
- **calculate_lod_recommendations**: Suggests which Level of Detail (LOD) model should be used based on an object's distance and screen presence
- **test_object_visibility**: Determines if a specific object is within the visible volume of the camera frustum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Field of View & Frustum Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the frustum geometry for a camera with a 60 degree vertical FOV and a 16:9 aspect ratio."

**🤖 AI Agent:**
> The horizontal FOV is 87.5 degrees. At 10m, the frustum width is 11.55m and height is 6.50m. At 50m, the width is 57.73m and height is 32.47m.

---

**👤 You:**
> "Is an object at position {x: 10, y: 5, z: 20} visible if the camera is at {x: 0, y: 0, z: 0} facing {x: 0, y: 0, z: 1} with a 90 degree vertical FOV and 1.77 aspect ratio?"

**🤖 AI Agent:**
> Yes, the object is within the visible frustum at a distance of 22.91 units.

---

**👤 You:**
> "What is the culling efficiency if there are 1000 total objects and 450 are outside the frustum?"

**🤖 AI Agent:**
> The culling efficiency is 0.45, with 450 objects successfully culled.


## ❓ FAQ

**Q: How can I check if a specific 3D object is visible to the camera?**
You can use the `test_object_visibility` tool. Provide the camera position, direction, object position, and frustum parameters to receive a boolean visibility result.

**Q: Can this tool help with LOD optimization?**
Yes, the `calculate_lod_recommendations` tool calculates the estimated screen percentage of an object to suggest the most efficient LOD level.

**Q: What kind of geometry data can I retrieve?**
The `calculate_frustum_geometry` tool provides the horizontal FOV, dimensions (width and height) at specific distances, and the visible surface area at those distances.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/field-of-view-frustum-calculator](https://vinkius.com/ai-agent-connect/field-of-view-frustum-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Field of View & Frustum Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `field-of-view-frustum-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Field of View & Frustum Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "field-of-view-frustum-calculator": {
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
