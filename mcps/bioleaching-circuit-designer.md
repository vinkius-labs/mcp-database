# Bioleaching Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bioleaching-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design bioleaching circuits by calculating reactor volumes, aeration, and retention times.

## Description
This MCP server provides specialized engineering tools for designing sulfide ore bioleaching operations. It allows engineers to model both heap and tank leaching configurations by analyzing mineralogy, bacterial kinetics, and temperature profiles. Use `calculate_heap_design` for large-scale pile operations, `calculate_tank_design` for stirred-tank reactors, and `compare_leaching_modes` to evaluate the trade-offs between different leaching methods. The server also includes `validate_microbial_viability` to ensure operating temperatures align with biological kinetic constraints.


## Available Tools (4)
- **calculate_heap_design**: Calculates the physical requirements for a heap leaching operation
- **calculate_tank_design**: Calculates the sizing and aeration for stirred-tank reactor bioleaching
- **compare_leaching_modes**: Compares the efficiency and requirements of heap vs. tank leaching
- **validate_microbial_viability**: Checks if the provided temperature and kinetic activity are compatible with known biological thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bioleaching Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the requirements for a heap leaching operation with 5000 tonnes of ore, a bacterial activity of 0.05, and a temperature of 35 degrees Celsius."

**🤖 AI Agent:**
> The heap design requires a reactor volume of 12500 m3, an aeration rate of 450 m3/h, and a retention time of 15 days.

---

**👤 You:**
> "What is the tank design for a throughput of 50 tonnes per hour at 45 degrees Celsius with a bacterial activity of 0.08?"

**🤖 AI Agent:**
> The stirred-tank reactor requires a volume of 850 m3, an aeration rate of 1200 m3/h, and a retention time of 17 hours.

---

**👤 You:**
> "Compare heap vs tank leaching for an ore with specific mineralogy, 0.04 bacterial activity, 30 degrees, and 10000 tonnes."

**🤖 AI Agent:**
> Heap leaching requires 25000 m3 volume, while tank leaching requires 4200 m3. Tank leaching offers 25% higher efficiency for this specific profile.


## ❓ FAQ

**Q: How do I calculate the aeration needed for my heap?**
You can use the `calculate_heap_design` tool. Provide the mineralogy JSON, bacterial activity, target temperature, and total ore mass to receive the required aeration rate.

**Q: Can I compare heap and tank leaching efficiency?**
Yes, the `compare_leaching_modes` tool evaluates the trade-offs between heap and tank methods based on your specific ore profile and kinetic requirements.

**Q: How do I check if my temperature is safe for the bacteria?**
Use the `validate_microbial_viability` tool with your target temperature and bacterial activity to check for biological compatibility and risk levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bioleaching-circuit-designer](https://vinkius.com/ai-agent-connect/bioleaching-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bioleaching Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bioleaching-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bioleaching Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bioleaching-circuit-designer": {
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
