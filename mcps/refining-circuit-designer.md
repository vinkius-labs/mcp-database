# Refining Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/refining-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design optimal metal refining circuits by selecting methods and sizing equipment.

## Description
This MCP server provides specialized tools for metallurgical engineering. It allows users to determine the best refining approach by using `select_refining_method` to choose between fire refining and electrorefining. Once a method is chosen, users can use `calculate_equipment_sizing` to determine the necessary volume and footprint, or `estimate_recovery_efficiency` to predict metal loss. The `analyze_circuit_feasibility` tool provides a high-level check to ensure throughput and purity requirements are achievable.


## Available Tools (4)
- **analyze_circuit_feasibility**: Performs a high-level assessment of whether the proposed design can realistically meet the user's goals
- **calculate_equipment_sizing**: Estimates the physical scale required for the refining equipment
- **estimate_recovery_efficiency**: Predicts the percentage of target metal that will be successfully recovered
- **select_refining_method**: Determines whether fire refining or electrorefining is the appropriate method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refining Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I use fire refining or electrorefining for a 95% purity feed with a throughput of 50 tonnes per hour?"

**🤖 AI Agent:**
> Fire refining is the recommended method for this throughput and purity level.

---

**👤 You:**
> "What is the required volume for an electrorefining setup with 10 tonnes per hour throughput?"

**🤖 AI Agent:**
> The required capacity volume for the electrolytic cell is 150 cubic meters.

---

**👤 You:**
> "Is it feasible to reach 99.99% purity with a 100 tonnes per hour throughput?"

**🤖 AI Agent:**
> No, the required throughput exceeds the maximum capacity for the high-precision electrorefining method needed for that purity.


## ❓ FAQ

**Q: How do I choose between fire refining and electrorefining?**
Use the `select_refining_method` tool. It evaluates your feed purity, target purity, and throughput to recommend the most suitable method.

**Q: Can I estimate the physical size of my furnace?**
Yes, the `calculate_equipment_sizing` tool provides the required capacity volume and footprint area based on your selected method and throughput.

**Q: How accurate are the recovery estimates?**
The `estimate_recovery_efficiency` tool provides a mathematical prediction of recovery rates and identifies the primary loss mechanism, such as slag entrapment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/refining-circuit-designer](https://vinkius.com/ai-agent-connect/refining-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refining Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refining-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refining Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refining-circuit-designer": {
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
