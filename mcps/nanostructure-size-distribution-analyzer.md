# Nanostructure Size Distribution Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nanostructure-size-distribution-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates nanoparticle size distribution metrics from DLS and TEM data.

## Description
This MCP server provides specialized statistical tools for nanoparticle characterization. It allows AI agents to process Dynamic Light Scattering (DLS) and Transmission Electron Microscopy (TEM) data to determine critical metrics like mean size, polydispersity index (PDI), and distribution width. Use `analyze_dls_data` for hydrodynamic sizing from intensity moments, `analyze_tem_data` for physical diameter counts, and `compare_characterization` to identify the difference between hydrodynamic and physical sizes.


## Available Tools (4)
- **analyze_dls_data**: Calculates size distribution metrics from DLS measurement sets
- **analyze_tem_data**: Calculates size distribution metrics from direct TEM measurements
- **compare_characterization**: Compares DLS and TEM results to identify differences
- **get_distribution_summary**: Provides a high-level descriptive summary of a specific distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nanostructure Size Distribution Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these TEM diameters: [12.5, 13.2, 11.8, 12.9, 12.1]"

**🤖 AI Agent:**
> The average physical diameter is 12.5 nm with a Polydispersity Index of 0.04.

---

**👤 You:**
> "What is the difference between my DLS and TEM results? DLS: {"meanSize": 25.0, "pdi": 0.1} TEM: {"meanSize": 18.0, "pdi": 0.05}"

**🤖 AI Agent:**
> The size difference is 7.0 nm, suggesting a surface layer thickness of approximately 7.0 nm.

---

**👤 You:**
> "Get a summary for these sizes using a log-normal model: [5.0, 5.5, 6.0]"

**🤖 AI Agent:**
> For the log-normal distribution, the mode is 5.45, the median is 5.5, and the mean is 5.48.


## ❓ FAQ

**Q: How do I analyze DLS data?**
Provide the intensity-weighted moments as a JSON string to the `analyze_dls_data` tool.

**Q: Can I compare DLS and TEM results?**
Yes, use the `compare_characterization` tool by providing the output objects from both DLS and TEM analyses.

**Q: What statistical models are supported?**
The server supports log-normal and normal distribution models via the `get_distribution_summary` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nanostructure-size-distribution-analyzer](https://vinkius.com/ai-agent-connect/nanostructure-size-distribution-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nanostructure Size Distribution Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nanostructure-size-distribution-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nanostructure Size Distribution Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nanostructure-size-distribution-analyzer": {
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
