# Crystal Field Theory Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crystal-field-theory-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate electronic configurations, CFSE, magnetic moments, and color predictions for transition metal complexes.

## Description
This MCP server provides a suite of computational tools for analyzing transition metal complexes using Crystal Field Theory (CFT). It allows AI agents to determine the electronic structure, stability, and physical properties of coordination compounds. By using `calculate_electronic_structure`, agents can identify spin states and orbital occupancy. Subsequent tools like `calculate_stabilization_energy` and `calculate_magnetic_properties` provide deep insights into the thermodynamic stability and magnetic behavior of the complex, while `predict_optical_properties` estimates the observed color based on d-to-d electronic transitions.


## Available Tools (4)
- **calculate_electronic_structure**: Determines the orbital splitting pattern and the resulting electronic configuration (spin state and occupancy)
- **calculate_magnetic_properties**: Determines the magnetic behavior and magnitude of the complex
- **calculate_stabilization_energy**: Calculates the net stability gain provided by the specific electron arrangement
- **predict_optical_properties**: Predicts the color of the complex based on light absorption


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crystal Field Theory Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the electronic structure of an Fe3+ ion in an octahedral field with a splitting energy of 20000?"

**🤖 AI Agent:**
> The Fe3+ ion in an octahedral field with a splitting energy of 20000 results in a high-spin configuration with 5 unpaired electrons.

---

**👤 You:**
> "Calculate the magnetic properties for a low-spin d6 octahedral complex."

**🤖 AI Agent:**
> A low-spin d6 octahedral complex has 0 unpaired electrons and is diamagnetic.

---

**👤 You:**
> "What color would a complex be if it absorbs light at 520 nm?"

**🤖 AI Agent:**
> A complex that absorbs light at 520 nm (green) will appear red.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can determine the electronic configuration, spin state, Crystal Field Stabilization Energy (CFSE), magnetic moment, and predicted color of transition metal complexes using `calculate_electronic_structure` and its companion tools.

**Q: Does it support different geometries?**
Yes, the server supports octahedral, tetrahedral, and square planar geometries via the `calculate_electronic_structure` tool.

**Q: How do I determine if a complex is paramagnetic?**
Use the `calculate_magnetic_properties` tool after obtaining the electronic structure; it will return whether the complex is paramagnetic or diamagnetic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crystal-field-theory-calculator](https://vinkius.com/ai-agent-connect/crystal-field-theory-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crystal Field Theory Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crystal-field-theory-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crystal Field Theory Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crystal-field-theory-calculator": {
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
