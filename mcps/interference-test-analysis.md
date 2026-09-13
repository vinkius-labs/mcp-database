# Interference Test Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/interference-test-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geoscience](../categories/geoscience.md)

Analyzes hydraulic communication and reservoir properties between wells.

## Description
This MCP server provides advanced reservoir engineering tools to analyze interference tests. It uses the diffusivity equation to determine interwell connectivity, permeability, and reservoir boundaries. Use `get_connectivity_profile` to evaluate hydraulic communication, `calculate_reservoir_properties` for physical reservoir characteristics, `detect_reservoir_boundaries` to find faults or edges, and `analyze_directional_permeability` to determine reservoir anisotropy.


## Available Tools (4)
- **calculate_reservoir_properties**: Derives fundamental physical properties of the reservoir using the diffusivity relationship
- **get_connectivity_profile**: Evaluates the hydraulic communication between a specific pair of wells
- **analyze_directional_permeability**: Determines the anisotropy of the reservoir by comparing responses across different orientations
- **detect_reservoir_boundaries**: Identifies the presence and location of reservoir limits such as faults or edges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Interference Test Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the connectivity between well A-1 and observation well B-2."

**🤖 AI Agent:**
> The connectivity index between well A-1 and B-2 is 0.85 with a response delay of 12 hours, indicating strong hydraulic communication.

---

**👤 You:**
> "Are there any reservoir boundaries near the active well?"

**🤖 AI Agent:**
> A boundary was detected at an estimated distance of 450 meters from the active well.

---

**👤 You:**
> "What is the permeability of the reservoir?"

**🤖 AI Agent:**
> The calculated permeability is 150 mD with a transmissibility of 2500 mD-ft.


## ❓ FAQ

**Q: How do I check if two wells are connected?**
You can use the `get_connectivity_profile` tool to evaluate the hydraulic communication between a specific active well and an observation well.

**Q: Can this tool detect faults in the reservoir?**
Yes, the `detect_reservoir_boundaries` tool identifies the presence and estimated distance of reservoir limits like faults.

**Q: How is permeability calculated?**
The `calculate_reservoir_properties` tool derives permeability by analyzing the pressure response relative to rate changes using the diffusivity equation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/interference-test-analysis](https://vinkius.com/en/ai-agent-connect/interference-test-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Interference Test Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `interference-test-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Interference Test Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "interference-test-analysis": {
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
