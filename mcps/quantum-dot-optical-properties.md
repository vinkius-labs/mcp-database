# Quantum Dot Optical Properties MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/quantum-dot-optical-properties)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate quantum dot band gaps, emission wavelengths, and confinement energies.

## Description
This MCP server provides precise calculations for the optical characteristics of semiconductor quantum dots. By applying quantum confinement equations and the effective mass approximation, it allows AI agents to determine the `bandGap`, `emissionWavelength`, and `confinementEnergy` for specific materials like CdSe or InP. Use `calculate_optical_properties` for a full profile, `get_confinement_energy` to isolate the energy shift, or `predict_emission_color` to find the visible color of a dot based on its diameter.


## Available Tools (4)
- **predict_emission_color**: Translates the calculated wavelength into a human-readable color description
- **calculate_optical_properties**: Provides a complete profile of the quantum dot's optical characteristics
- **compare_materials_for_size**: Compares how different materials respond to the same physical diameter
- **get_confinement_energy**: Isolates the specific energy shift caused by quantum confinement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quantum Dot Optical Properties** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the optical properties of a 5nm CdSe quantum dot using the spherical-ema model?"

**🤖 AI Agent:**
> For a 5nm CdSe quantum dot, the band gap is 2.55 eV, the emission wavelength is 486.3 nm, and the confinement energy is 0.42 eV.

---

**👤 You:**
> "What color will a 3nm InP quantum dot emit?"

**🤖 AI Agent:**
> A 3nm InP quantum dot will emit blue light.

---

**👤 You:**
> "Compare the band gap of CdSe and PbS at a diameter of 6nm."

**🤖 AI Agent:**
> At 6nm, CdSe has a band gap of 2.12 eV, while PbS has a band gap of 0.95 eV.


## ❓ FAQ

**Q: What parameters are required for calculations?**
You must provide the dot diameter in nanometers, the semiconductor material identifier, and the specific confinement model to be used.

**Q: Can I compare different materials at the same size?**
Yes, you can use the `compare_materials_for_size` tool to see how different materials respond to the same physical diameter.

**Q: How is the emission color determined?**
The color is determined by mapping the calculated emission wavelength to the visible light spectrum using the `predict_emission_color` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/quantum-dot-optical-properties](https://vinkius.com/ai-agent-connect/quantum-dot-optical-properties)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quantum Dot Optical Properties** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quantum-dot-optical-properties` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quantum Dot Optical Properties** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quantum-dot-optical-properties": {
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
