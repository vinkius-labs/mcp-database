# Polymerization Degree Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/polymerization-degree-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate degree of polymerization, repeat units, and PDI for polymer chains.

## Description
This MCP server provides specialized chemical engineering tools to analyze polymer structures. It allows AI agents to determine the degree of polymerization ($DP_n$ and $DP_w$), calculate the number of repeat units, and determine the Polydispersity Index (PDI) using monomeric and molecular weight data. Use `get_molecular_distribution_summary` for a complete overview of molecular characteristics or `calculate_pdi` to assess the breadth of molecular weight distribution.


## Available Tools (4)
- **calculate_dp_from_mn**: Determines the number-average degree of polymerization using the number-average molecular weight and the monomer mass
- **calculate_dp_from_mw**: Determines the weight-average degree of polymerization
- **calculate_pdi**: Calculates the Polydispersity Index to understand the breadth of the molecular weight distribution
- **get_molecular_distribution_summary**: Provides a comprehensive overview of the polymer's molecular characteristics from all available weight averages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polymerization Degree Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the degree of polymerization for a polymer with a monomer weight of 44 and a number-average molecular weight of 4400."

**🤖 AI Agent:**
> The degree of polymerization is 100 with 100 repeat units.

---

**👤 You:**
> "What is the PDI if the weight-average molecular weight is 5000 and the number-average molecular weight is 2500?"

**🤖 AI Agent:**
> The Polydispersity Index (PDI) is 2.0.

---

**👤 You:**
> "Provide a summary for a polymer with monomer weight 100, Mn 10000, and Mw 12000."

**🤖 AI Agent:**
> The polymer has a number-average DP of 100, a weight-average DP of 120, and a PDI of 1.2.


## ❓ FAQ

**Q: What is the Polydispersity Index (PDI)?**
The PDI is a measure of the distribution of molecular masses in a polymer sample. A PDI of 1 indicates a monodisperse sample where all chains are the same length.

**Q: How do I calculate the degree of polymerization?**
You can use the `calculate_dp_from_mn` tool by providing the monomer weight and the number-average molecular weight.

**Q: Can I get a full summary of my polymer sample?**
Yes, the `get_molecular_distribution_summary` tool provides a comprehensive overview including $DP_n$, $DP_w$, and PDI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/polymerization-degree-calculator](https://vinkius.com/ai-agent-connect/polymerization-degree-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polymerization Degree Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polymerization-degree-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polymerization Degree Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polymerization-degree-calculator": {
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
