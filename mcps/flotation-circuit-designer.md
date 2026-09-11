# Flotation Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flotation-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design mineral flotation circuits by modeling kinetic separation based on ore characteristics.

## Description
This MCP server provides specialized engineering tools for mineral processing. It allows AI agents to design complete flotation circuits by calculating physical parameters like residence time and cell count. Using `calculate_circuit_requirements`, agents can determine the necessary circuit configuration. The server also supports balancing recovery and grade through `optimize_stage_distribution`, verifying feasibility with `validate_liberation_efficiency`, and predicting final outcomes via `simulate_circuit_performance`.


## Available Tools (4)
- **calculate_circuit_requirements**: Determines the fundamental physical parameters of the flotation circuit based on mineral properties and goals
- **optimize_stage_distribution**: Adjusts the proportion of the circuit dedicated to Rougher, Scavenger, and Cleaner stages to balance recovery vs. grade
- **simulate_circuit_performance**: Predicts the final concentrate grade and recovery for a specific circuit configuration
- **validate_liberation_efficiency**: Assesses if the proposed liberation size is sufficient to achieve the recovery target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flotation Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the requirements for a circuit with a flow rate of 500 m3/h, a liberation size of 75 microns, and a recovery target of 85%."

**🤖 AI Agent:**
> The circuit requires a total residence time of 120 minutes, consisting of 5 cells with a total volume of 1000 m3, configured with rougher, scavenger, and cleaner stages.

---

**👤 You:**
> "Is it feasible to achieve 90% recovery with a liberation size of 50 microns for this mineralogy?"

**🤖 AI Agent:**
> Yes, the estimated recovery at 50 microns is 92%, making the 90% target feasible.

---

**👤 You:**
> "Predict the performance of a circuit optimized for grade."

**🤖 AI Agent:**
> The predicted final grade is 88% with a recovery of 82% and a mass pull of 5.5%.


## ❓ FAQ

**Q: How do I determine the number of flotation cells needed?**
You can use the `calculate_circuit_requirements` tool. By providing the mineralogy, liberation size, recovery target, and flow rate, the tool calculates the total residence time and the required number of cells.

**Q: Can I optimize the circuit for higher purity?**
Yes. Use the `optimize_stage_distribution` tool and set the priority to 'grade' to increase the proportion of the cleaner stage.

**Q: How can I check if my recovery target is realistic?**
The `validate_liberation_efficiency` tool assesses if the proposed liberation size is sufficient to achieve your specific recovery target.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flotation-circuit-designer](https://vinkius.com/en/ai-agent-connect/flotation-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flotation Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flotation-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flotation Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flotation-circuit-designer": {
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
