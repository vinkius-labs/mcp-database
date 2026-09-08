# Magnetic Separation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/magnetic-separation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design optimal magnetic separation circuits by calculating field strength, equipment selection, and efficiency.

## Description
This MCP server provides specialized engineering tools for designing magnetic separation circuits. It allows users to determine optimal magnetic field strength, select the correct equipment type (such as LIMS, MIMS, WHIMS, or HGMS), and predict separation efficiency based on mineral susceptibility, particle size, and throughput. Use `design_separation_circuit` to generate a full design, `evaluate_equipment_suitability` to verify machinery, or `predict_efficiency_loss` to account for physical factors like particle size and medium type.


## Available Tools (4)
- **compare_wet_vs_dry_parameters**: Provides a comparative analysis of how the separation performance would change if switching between wet and dry modes
- **design_separation_circuit**: Generates a complete magnetic separation design including field strength, equipment type, and predicted efficiency
- **evaluate_equipment_suitability**: Determines if a specific piece of magnetic equipment is capable of handling the provided mineral characteristics
- **predict_efficiency_loss**: Calculates the potential loss of target minerals due to specific environmental or physical factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magnetic Separation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a magnetic separation circuit for a mineral with 0.05 susceptibility, 50 micron particle size, and 100 tons per hour throughput using wet separation."

**🤖 AI Agent:**
> The recommended design requires a magnetic field strength of 0.8 Tesla using WHIMS equipment, with a predicted separation efficiency of 94.5%.

---

**👤 You:**
> "Is a LIMS equipment suitable for a mineral with 0.5 susceptibility and 200 micron particle size?"

**🤖 AI Agent:**
> Yes, LIMS is suitable for this mineral profile with a high confidence score.

---

**👤 You:**
> "Compare wet vs dry separation for a mineral with 0.1 susceptibility and 40 micron particle size."

**🤖 AI Agent:**
> Wet separation is recommended for this fine particle size to maximize efficiency, providing a significant advantage over dry separation.


## ❓ FAQ

**Q: How do I design a new separation circuit?**
You can use the `design_separation_circuit` tool by providing the mineral susceptibility, particle size, throughput, and whether the process is wet or dry.

**Q: Can I check if my equipment is suitable for a specific ore?**
Yes, use the `evaluate_equipment_suitability` tool to check if a specific equipment type matches your mineral's susceptibility and particle size.

**Q: How does particle size affect my efficiency?**
Smaller particles can lead to higher losses. You can use `predict_efficiency_loss` to calculate how particle size and the separation medium impact your results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/magnetic-separation-design](https://vinkius.com/ai-agent-connect/magnetic-separation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magnetic Separation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `magnetic-separation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magnetic Separation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magnetic-separation-design": {
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
