# Crystallite Size Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crystallite-size-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Analyze XRD data to determine crystallite size, microstrain, and instrumental broadening.

## Description
This MCP server provides specialized tools for X-ray Diffraction (XRD) analysis. It allows AI agents to calculate physical characteristics of crystalline materials using the Scherrer equation and Williamson-Hall analysis. Users can determine crystallite size with `calculate_scherrer_size`, isolate lattice distortions using `analyze_microstrain`, and account for equipment effects via `estimate_instrumental_broadening`. For a complete material profile, `perform_williamson_hall_analysis` combines these factors to provide both average size and microstrain.


## Available Tools (4)
- **analyze_microstrain**: Separates the microstrain component from the total peak broadening
- **calculate_scherrer_size**: Calculates the crystallite size using the Scherrer equation
- **estimate_instrumental_broadening**: Determines the width contribution caused by the measurement equipment
- **perform_williamson_hall_analysis**: Conducts a comprehensive analysis by combining size and strain effects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crystallite Size Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the crystallite size for a peak with width 0.5, wavelength 0.154, and theta 15.0."

**🤖 AI Agent:**
> The calculated crystallite size is 25.4 nm.

---

**👤 You:**
> "What is the microstrain if the observed width is 0.8, the size-induced width is 0.5, and theta is 20.0?"

**🤖 AI Agent:**
> The estimated microstrain is 0.0012.

---

**👤 You:**
> "Get the instrumental broadening for a standard lab XRD."

**🤖 AI Agent:**
> The instrumental broadening width is 0.045.


## ❓ FAQ

**Q: What is the primary use of this tool?**
It is used to calculate crystallite size and microstrain from X-ray diffraction peak data.

**Q: How do I account for my XRD machine's specific characteristics?**
You can use the `estimate_instrumental_broadening` tool with a standard profile like 'standard_lab_xrd' to find the equipment's width contribution.

**Q: Can I perform a full Williamson-Hall analysis?**
Yes, by providing multiple peak data points to the `perform_williamson_hall_analysis` tool, you can derive both size and strain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crystallite-size-calculator](https://vinkius.com/ai-agent-connect/crystallite-size-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crystallite Size Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crystallite-size-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crystallite Size Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crystallite-size-calculator": {
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
