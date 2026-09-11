# Seepage Analysis for Tailings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seepage-analysis-for-tailings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze seepage, phreatic surfaces, and exit gradients in tailings storage facilities.

## Description
This MCP server provides specialized engineering tools for analyzing water movement and stability risks in tailings storage facilities. It allows AI agents to calculate the phreatic surface, estimate total seepage volume, evaluate exit gradients at specific coordinates, and assess the effectiveness of drainage systems. By connecting to Vinkius Edge, agents can perform complex hydraulic calculations using facility geometry, material properties, and hydraulic conditions to ensure dam stability and liner performance.


## Available Tools (4)
- **estimate_seepage_volume**: 
- **evaluate_drainage_efficiency**: 
- **assess_exit_gradient**: 
- **calculate_phreatic_surface**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seepage Analysis for Tailings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated seepage volume for a facility with a liner integrity of 0.9?"

**🤖 AI Agent:**
> The total flow rate for the facility is 0.045 m³/s with a seepage loss component of 0.002 m³/s.

---

**👤 You:**
> "Calculate the phreatic surface for the current geometry and hydraulic head."

**🤖 AI Agent:**
> The phreatic surface has been calculated. The maximum saturation depth is 12.5 meters and the saturation volume is 450.0 cubic meters.

---

**👤 You:**
> "Is the exit gradient at the downstream toe within safe limits?"

**🤖 AI Agent:**
> The exit gradient at the specified coordinates is 0.05, which is well below the critical threshold. The stability status is Stable.


## ❓ FAQ

**Q: How can I check the stability risk at the dam toe?**
You can use the `assess_exit_gradient` tool to evaluate the hydraulic gradient at specific coordinates, which helps identify risks of piping or internal erosion.

**Q: Can this tool account for liner leakage?**
Yes, the `estimate_seepage_volume` tool includes a liner integrity parameter to account for how efficiently the installed liner prevents water loss.

**Q: How do I determine the saturation boundary?**
Use the `calculate_phreatic_surface` tool to determine the location and shape of the saturation boundary based on facility geometry and hydraulic conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seepage-analysis-for-tailings](https://vinkius.com/en/ai-agent-connect/seepage-analysis-for-tailings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seepage Analysis for Tailings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seepage-analysis-for-tailings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seepage Analysis for Tailings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seepage-analysis-for-tailings": {
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
