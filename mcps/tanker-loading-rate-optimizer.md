# Tanker Loading Rate Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tanker-loading-rate-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimizes tanker loading rates by balancing vessel capacity, shore infrastructure, and safety constraints.

## Description
This MCP server provides specialized tools for maritime logistics and terminal operations. It calculates safe loading speeds by accounting for vessel capacity, shore tank availability, and pipeline limits. It specifically addresses critical safety factors such as Vapor Recovery Unit (VRU) capacity and static electricity prevention during initial filling. Users can use `get_maximum_safe_loading_rate` to find optimal speeds, `calculate_line_fill_metrics` to estimate pipeline preparation, `analyze_backpressure_risk` to prevent manifold damage, and `validate_loading_plan` for a complete operational safety check.


## Available Tools (4)
- **analyze_backpressure_risk**: Evaluates if the requested loading rate will cause pressure to exceed safe limits at the vessel connection
- **calculate_line_fill_metrics**: Estimates the time and volume required to fill the transfer pipeline before vessel loading commences
- **get_maximum_safe_loading_rate**: Determines the highest permissible loading rate that respects all safety and infrastructure constraints
- **validate_loading_plan**: Performs a holistic check of a proposed loading operation against all operational parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tanker Loading Rate Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum safe loading rate for a 50,000 m3 vessel with 60,000 m3 available in the shore tank, a 1,500 m3/h pipeline, and a 1,200 m3/h VRU capacity?"

**🤖 AI Agent:**
> The maximum safe loading rate is 1,200 m3/h, limited by the VRU capacity.

---

**👤 You:**
> "How long will it take to fill a 500 m3 pipeline if I am loading at 250 m3/h?"

**🤖 AI Agent:**
> It will take 2 hours to fill the pipeline, using 500 m3 of product.

---

**👤 You:**
> "Is a loading rate of 1,500 m3/h safe for a 100m pipeline with a 200mm diameter and a 5 bar pressure limit?"

**🤖 AI Agent:**
> No, the estimated pressure is 5.8 bar, which exceeds the 5 bar limit.


## ❓ FAQ

**Q: How does the tool handle static electricity safety?**
The `get_maximum_safe_loading_rate` tool includes an `isInitialFilling` parameter. When active, it enforces low-velocity thresholds to prevent static charge buildup during initial contact.

**Q: Can I check if my loading rate will damage the vessel manifold?**
Yes, you can use `analyze_backpressure_risk` to evaluate if the requested rate will cause pressure to exceed the manifold's maximum allowable limit.

**Q: What happens if the Vapor Recovery Unit (VRU) is a bottleneck?**
The `get_maximum_safe_loading_rate` tool considers the `vrpCapacity` input. If the VRU capacity is lower than the pipeline capacity, the tool will return the VRU limit as the constraint reason.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tanker-loading-rate-optimizer](https://vinkius.com/en/ai-agent-connect/tanker-loading-rate-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tanker Loading Rate Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tanker-loading-rate-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tanker Loading Rate Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tanker-loading-rate-optimizer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
