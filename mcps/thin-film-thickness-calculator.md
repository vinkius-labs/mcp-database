# Thin Film Thickness Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/thin-film-thickness-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate thin film thickness, refractive index, and extinction coefficient from interferometry and ellipsometry data.

## Description
This MCP server provides specialized tools for thin-film characterization. It allows AI agents to process optical measurement data to determine physical properties of materials. Use `calculate_single_layer_thickness` to find the thickness of a uniform film using interference patterns. Use `analyze_ellipsometry_data` to extract both thickness and complex refractive index (n and k) from polarization measurements. For complex stacks, `calculate_multilayer_thickness` resolves individual layer thicknesses. You can also use `validate_optical_constants` to check if provided n and k values are physically plausible.


## Available Tools (4)
- **analyze_ellipsometry_data**: Analyzes ellipsometry data to find thickness and optical constants (n and k)
- **calculate_multilayer_thickness**: Calculates the thickness of individual layers in a complex multi-stack system
- **calculate_single_layer_thickness**: Calculates the thickness of a single uniform thin film based on interference data
- **validate_optical_constants**: Validates if provided refractive index and extinction coefficient are physically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thin Film Thickness Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the thickness of a single uniform thin film with wavelengths [500, 510, 520] and intensities [0.8, 0.7, 0.6], given a refractive index of 1.5 and substrate index of 1.0?"

**🤖 AI Agent:**
> The calculated thickness of the thin film is 125.4 nm with an uncertainty of 0.2 nm.

---

**👤 You:**
> "Analyze this ellipsometry data: psi [10, 12], delta [5, 7], wavelengths [550, 560], and substrate index 1.5."

**🤖 AI Agent:**
> The film thickness is 45.2 nm, with a refractive index of 1.45 and an extinction coefficient of 0.01 at 550 nm.

---

**👤 You:**
> "Is a refractive index of 2.5 and extinction coefficient of 0.001 plausible for a dielectric material?"

**🤖 AI Agent:**
> Yes, these values are physically plausible for a dielectric material.


## ❓ FAQ

**Q: What kind of data is required for thickness calculation?**
For single layers, you need arrays of wavelengths and interference intensities. For ellipsometry, you need psi and delta values along with wavelengths.

**Q: Can I analyze multi-layer stacks?**
Yes, the `calculate_multilayer_thickness` tool is designed to resolve individual thicknesses within a complex multi-stack system.

**Q: How do I verify if my optical constants are correct?**
You can use the `validate_optical_constants` tool to check if the refractive index and extinction coefficient are physically plausible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/thin-film-thickness-calculator](https://vinkius.com/ai-agent-connect/thin-film-thickness-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thin Film Thickness Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thin-film-thickness-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thin Film Thickness Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thin-film-thickness-calculator": {
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
