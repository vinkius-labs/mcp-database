# Particle in a Box Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/particle-in-a-box-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Simulate quantum mechanics for particles in 1D, 2D, and 3D rigid potential wells.

## Description
This MCP server provides tools to solve fundamental quantum mechanics problems for particles confined in rigid potential wells. You can use `calculate_energy_state` to find discrete energy levels, `get_wavefunction_amplitude` to find the wavefunction value at specific coordinates, `get_probability_density` to determine the likelihood of finding a particle at a point, and `list_energy_spectrum` to view a range of available energy states. It supports 1D, 2D, and 3D configurations.


## Available Tools (4)
- **calculate_energy_state**: Determines the specific energy level for a particle in a given box dimension and state
- **get_probability_density**: Calculates the probability density at a specific point in space
- **get_wavefunction_amplitude**: Calculates the value of the wavefunction at a specific spatial coordinate
- **list_energy_spectrum**: Provides a range of available energy levels for a particle within a specific box configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Particle in a Box Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the energy level for an electron in a 1D box of 1nm length with n=1?"

**🤖 AI Agent:**
> The energy level for an electron in a 1nm 1D box at n=1 is approximately 6.025e-19 Joules.

---

**👤 You:**
> "Calculate the probability density at x=0.5 for a 1D box of 1m length, mass 1kg, n=1."

**🤖 AI Agent:**
> The probability density at x=0.5 is 0.4 Joules/m^2.

---

**👤 You:**
> "List the first few energy levels for a 2D box with Lx=1, Ly=1, mass=1, up to n=2."

**🤖 AI Agent:**
> The energy levels are: nx=1, ny=1: 1.0; nx=1, ny=2: 2.0; nx=2, ny=1: 2.0; nx=2, ny=2: 4.0.


## ❓ FAQ

**Q: What dimensions are supported?**
The server supports 1D, 2D, and 3D rigid potential wells.

**Q: How do I find the energy of a specific state?**
Use the `calculate_energy_state` tool by providing the dimension, box dimensions, particle mass, and quantum numbers.

**Q: Can I see multiple energy levels at once?**
Yes, you can use `list_energy_spectrum` to retrieve a range of energy levels up to a specified maximum quantum number.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/particle-in-a-box-calculator](https://vinkius.com/ai-agent-connect/particle-in-a-box-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Particle in a Box Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `particle-in-a-box-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Particle in a Box Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "particle-in-a-box-calculator": {
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
