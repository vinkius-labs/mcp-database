# Nanoparticle Surface Area Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nanoparticle-surface-area-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate specific surface area, surface atom fraction, and size distribution for nanoparticles.

## Description
This MCP server provides precise geometric and physical calculations for nanoparticle characterization. It allows AI agents to determine the specific surface area using `calculate_specific_surface_area`, estimate the percentage of atoms on the surface via `calculate_surface_atom_fraction`, and analyze populations of particles with `analyze_size_distribution`. It is designed for material scientists and researchers working with nanoscale morphology.


## Available Tools (4)
- **analyze_size_distribution**: Calculates average physical properties across a population of particles with varying sizes
- **calculate_specific_surface_area**: Calculates the specific surface area for a given particle shape and size
- **calculate_surface_atom_fraction**: Calculates the percentage of atoms located on the surface of the particle
- **get_morphology_constants**: Retrieves geometric scaling factors for a specific shape


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nanoparticle Surface Area Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the specific surface area of a sphere with a radius of 5nm and a density of 2.5 g/cm³?"

**🤖 AI Agent:**
> The specific surface area for the sphere is 0.24 m²/g.

---

**👤 You:**
> "What percentage of atoms are on the surface for a cube with a side length of 2nm and an atomic radius of 0.12nm?"

**🤖 AI Agent:**
> The surface atom percentage for this cube is 42.5%.

---

**👤 You:**
> "Find the geometric scaling factors for a cylinder."

**🤖 AI Agent:**
> The surface area factor is 2πr(h+r) and the volume factor is πr²h.


## ❓ FAQ

**Q: How do I calculate the specific surface area?**
You can use the `calculate_specific_surface_area` tool by providing the particle size, density, and the geometric shape.

**Q: Can I analyze a group of particles at once?**
Yes, the `analyze_size_distribution` tool calculates weighted average properties across a population of varying particle sizes.

**Q: What shapes are supported?**
The server supports sphere, cube, and cylinder geometries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nanoparticle-surface-area-analyzer](https://vinkius.com/ai-agent-connect/nanoparticle-surface-area-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nanoparticle Surface Area Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nanoparticle-surface-area-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nanoparticle Surface Area Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nanoparticle-surface-area-analyzer": {
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
