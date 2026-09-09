# Classification Efficiency Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/classification-efficiency-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Models classification efficiency for hydrocyclones and screens using partition curves and separation metrics.

## Description
This MCP server provides advanced mathematical modeling for mineral processing and particle separation. It allows AI agents to calculate partition curves, evaluate separation quality, and predict equipment performance for hydrocyclones and screens. Users can model the impact of the fish hook effect using `simulate_fish_hook_impact` or forecast stream distributions with `predict_equipment_performance`. The toolset includes `analyze_partition_curve` for generating probability distributions and `calculate_separation_metrics` for evaluating sharpness and efficiency.


## Available Tools (4)
- **analyze_partition_curve**: Generates the probability distribution for particle recovery across a range of sizes
- **calculate_separation_metrics**: Evaluates the quality of the classification based on feed and partition data
- **predict_equipment_performance**: Forecasts the resulting size distribution of the underflow and overflow streams
- **simulate_fish_hook_impact**: Predicts how the fish hook effect will alter the predicted recovery of fine particles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Classification Efficiency Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a partition curve for a cut size of 50 microns, a sharpness index of 1.5, and a bypass fraction of 0.1."

**🤖 AI Agent:**
> The generated partition curve shows a probability distribution centered around the 50 micron cut size, adjusted for the 0.1 bypass fraction.

---

**👤 You:**
> "What happens to the recovery if there is a fish hook effect at 20 microns with a magnitude of 0.05?"

**🤖 AI Agent:**
> The adjusted curve shows an increased recovery of fine particles near the 20 micron size due to the specified deviation.

---

**👤 You:**
> "Calculate the separation metrics for a feed distribution and a specific partition curve."

**🤖 AI Agent:**
> The calculated metrics show a sharpness of 1.4, a bypass of 0.08, and an overall efficiency of 85%.


## ❓ FAQ

**Q: How can I model the separation quality of my hydrocyclone?**
You can use `calculate_separation_metrics` after generating a partition curve with `analyze_partition_curve` to determine sharpness and efficiency.

**Q: What is the fish hook effect in classification?**
The fish hook effect is a deviation in the partition curve where fine particles are recovered unexpectedly. You can simulate this using `simulate_fish_hook_impact`.

**Q: Can I predict the output of my equipment?**
Yes, use `predict_equipment_performance` to forecast the resulting size distribution of both underflow and overflow streams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/classification-efficiency-model](https://vinkius.com/ai-agent-connect/classification-efficiency-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Classification Efficiency Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `classification-efficiency-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Classification Efficiency Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "classification-efficiency-model": {
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
