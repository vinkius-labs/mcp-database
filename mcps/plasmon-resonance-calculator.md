# Plasmon Resonance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/plasmon-resonance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-computing](../categories/scientific-computing.md)

Calculate surface plasmon resonance wavelength, extinction, and field enhancement for metallic nanoparticles.

## Description
This MCP server provides precise calculations for Surface Plasmon Resonance (SPR) in metallic nanoparticles using Mie theory approximations. It allows AI agents to determine the resonance wavelength, extinction coefficients (including absorption and scattering contributions), and electric field enhancement factors based on particle material, size, shape, and the surrounding medium's refractive index. Use `get_resonance_wavelength` to find peak wavelengths, `get_extinction_coefficient` for light attenuation, `get_field_enhancement` for surface field concentration, and `compare_material_performance` to evaluate different metals under identical conditions.


## Available Tools (4)
- **compare_material_performance**: 
- **get_extinction_coefficient**: 
- **get_field_enhancement**: 
- **get_resonance_wavelength**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plasmon Resonance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the resonance wavelength for a 50nm gold sphere in water?"

**🤖 AI Agent:**
> The resonance wavelength for a 50nm gold sphere in water (refractive index 1.33) is 530 nm.

---

**👤 You:**
> "Calculate the field enhancement for a silver nanorod with an aspect ratio of 3."

**🤖 AI Agent:**
> The electric field enhancement factor for the silver nanorod is 45.2, with the peak location at the tips.

---

**👤 You:**
> "Compare the extinction coefficient of gold and silver spheres of size 40nm in air."

**🤖 AI Agent:**
> For 40nm spheres in air, gold has an extinction coefficient of 0.015, while silver has a higher coefficient of 0.042.


## ❓ FAQ

**Q: What materials are supported for calculation?**
The calculator supports noble metals like gold and silver, as well as transition metals such as copper and aluminum.

**Q: How do I calculate the resonance for a nanorod?**
To calculate for a rod, use the `get_resonance_wavelength` tool and ensure you provide the `aspectRatio` parameter.

**Q: Can I compare different metals at once?**
Yes, you can use the `compare_material_performance` tool to evaluate multiple metals simultaneously under the same physical parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/plasmon-resonance-calculator](https://vinkius.com/ai-agent-connect/plasmon-resonance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plasmon Resonance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plasmon-resonance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plasmon Resonance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plasmon-resonance-calculator": {
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
