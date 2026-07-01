# Matrix 4x4 Transforms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matrix-4x4-transforms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Create, compose, and apply 3D transformation matrices with rotation representations and coordinate transformations for graphics and simulation applications.

## Description
This MCP server provides comprehensive tools for working with 4x4 transformation matrices in 3D graphics and simulation. Create translation, rotation (around X/Y/Z axes by angle), scale, and shear matrices. Compose multiple transforms by multiplying matrices in order. Transform a 3D point by a 4x4 matrix with perspective divide. Extract Euler angles from rotation matrix with gimbal lock warning. Convert between rotation matrix, quaternion, and axis-angle representations. Use tools like `create_translation_matrix`, `create_rotation_matrix`, `compose_transforms`, and `transform_point` to build complete transformation pipelines for model, view, and projection stages in graphics applications.


## Available Tools (11)
- **axis_angle_to_quaternion**: Convert axis-angle to a quaternion
- **compose_transforms**: Combine multiple transformation matrices into one composite matrix
- **create_rotation_matrix**: Generate a 4x4 rotation matrix around a specified axis
- **create_scale_matrix**: Generate a 4x4 scale matrix along axes
- **create_shear_matrix**: Generate a 4x4 shear matrix along axes
- **create_translation_matrix**: Generate a 4x4 transformation matrix for translating objects
- **matrix_to_euler_angles**: Extract Euler angles from a rotation matrix
- **quaternion_to_axis_angle**: Convert a quaternion to axis-angle representation
- **quaternion_to_rotation_matrix**: Convert a quaternion to a 3x3 rotation matrix
- **rotation_matrix_to_quaternion**: Convert a 3x3 rotation matrix to a quaternion
- **transform_point**: Apply a 4x4 matrix to a 3D point with perspective divide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matrix 4x4 Transforms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a translation matrix that moves an object 5 units along the x-axis, 3 units along the y-axis, and 2 units along the z-axis."

**🤖 AI Agent:**
> The translation matrix has been created with tx=5, ty=3, and tz=2. The bottom row of the 4x4 matrix contains [5, 3, 2, 1], and all other entries are zero except the diagonal which is 1.

---

**👤 You:**
> "Rotate a point (1, 2, 3) by 45 degrees around the Y-axis using a rotation matrix."

**🤖 AI Agent:**
> The rotation matrix for 45 degrees around the Y-axis has been applied to the point (1, 2, 3). The resulting transformed point is approximately (0.707, 2, 4.121) after the rotation transformation.

---

**👤 You:**
> "Convert the rotation matrix [[0.707, 0, 0.707], [0, 1, 0], [-0.707, 0, 0.707]] to Euler angles."

**🤖 AI Agent:**
> The rotation matrix converts to Euler angles [0°, 0°, 90°] with no gimbal lock detected. This represents a 90-degree rotation around the Z-axis.


## ❓ FAQ

**Q: What is homogeneous coordinates and why are they used?**
Homogeneous coordinates represent 3D points as 4D vectors [x, y, z, w]. This representation enables translation and projection operations to be expressed as linear transformations using 4x4 matrices. Points are converted back to 3D by dividing by the w-component (perspective divide) when w ≠ 1.

**Q: How do I compose multiple transformation matrices?**
Use the `compose_transforms` tool with an array of matrices in application order. The first listed matrix is applied first to the point. Composition uses right-to-left multiplication: if a point transforms first by matrix A then by matrix B, the composition is B × A.

**Q: What is gimbal lock and how does this tool handle it?**
Gimbal lock occurs when rotation axes align, causing loss of a degree of freedom. The `matrix_to_euler_angles` tool detects this condition and returns a `gimbal_lock` flag with an explanation. This helps identify problematic rotation sequences in your graphics pipeline.

**Q: Why use quaternions instead of rotation matrices?**
Quaternions avoid gimbal lock and are numerically stable for interpolation and composition. The `quaternion_to_rotation_matrix`, `quaternion_to_axis_angle`, and `axis_angle_to_quaternion` tools enable seamless conversion between quaternion and matrix representations for optimal performance in different scenarios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matrix-4x4-transforms](https://vinkius.com/mcp/matrix-4x4-transforms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Matrix 4x4 Transforms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `matrix-4x4-transforms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Matrix 4x4 Transforms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "matrix-4x4-transforms": {
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
