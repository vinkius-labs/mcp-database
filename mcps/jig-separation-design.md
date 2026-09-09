# Jig Separation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/jig-separation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Technical tool for designing jigging circuits based on mineral density and throughput.

## Description
This MCP server provides specialized tools for mineral processing engineers to design efficient gravity separation circuits. By inputting mineral density differences and particle size ranges, users can use `get_circuit_dimensions` to determine physical footprint, `calculate_pulsation_parameters` for optimal bed movement, `design_bed_configuration` for bed and ragging specifications, and `configure_hutch_water_flow` to stabilize the separation process.


## Available Tools (4)
- **calculate_pulsation_parameters**: Determines the optimal frequency and stroke length for the jigging action
- **configure_hutch_water_flow**: Determines the amount of hutch water needed to stabilize the bed and control suction
- **design_bed_configuration**: Defines the thickness of the mineral bed and the necessary ragging layer
- **get_circuit_dimensions**: Calculates the physical footprint and required volume of the jig to handle a specific throughput


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jig Separation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the jig dimensions for a throughput of 500 m3/h with particle sizes between 0.5mm and 5mm."

**🤖 AI Agent:**
> The jig requires a length of 4.5m, a width of 3.0m, a total surface area of 13.5m², and a required bed volume of 27.0m³.

---

**👤 You:**
> "What are the pulsation parameters for a density difference of 1.2 g/cm³ and particle sizes from 0.2mm to 2mm?"

**🤖 AI Agent:**
> The optimal pulsation frequency is 145 pulses per minute, with a stroke length of 12mm and a bed fluidization index of 0.85.

---

**👤 You:**
> "Design the bed configuration for a 2.0mm max particle size and 1.0 g/cm³ density difference at 300 m3/h throughput."

**🤖 AI Agent:**
> The recommended bed depth is 0.45m, the ragging thickness should be 4.0mm, and the ragging material density should be 3.5 g/cm³.


## ❓ FAQ

**Q: What parameters are required for circuit dimensioning?**
To use `get_circuit_dimensions`, you must provide the target throughput, the minimum particle size, and the maximum particle size in the feed.

**Q: How does the tool handle ragging selection?**
The `design_bed_configuration` tool calculates the necessary ragging thickness based on the largest particle size and recommends a suitable ragging material density.

**Q: Can I calculate water requirements for the hutch?**
Yes, the `configure_hutch_water_flow` tool determines the required hutch water rate and suction control factor based on particle size and bed depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/jig-separation-design](https://vinkius.com/ai-agent-connect/jig-separation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jig Separation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jig-separation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jig Separation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jig-separation-design": {
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
