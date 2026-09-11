# Perforating Gun Selection Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/perforating-gun-selection-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Select optimal perforating gun systems based on casing, formation, and conveyance constraints.

## Description
This MCP server provides an intelligent decision engine for oil and gas completion operations. It allows AI agents to calculate penetration depth, evaluate system capacity for wireline or TCP deployment, and recommend the best gun configuration. By using `select_optimal_system`, agents can match casing diameters and formation hardness to specific shaped charge performance metrics.


## Available Tools (4)
- **calculate_system_capacity**: Determines if a specific gun system can be safely deployed based on the conveyance method
- **evaluate_penetration_capability**: Predicts the effective penetration depth based on formation resistance and charge performance
- **get_gun_performance**: Retrieves specific performance metrics for a selected charge type
- **select_optimal_system**: Recommends the best gun configuration by matching casing constraints and formation requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perforating Gun Selection Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend a gun system for a 7-inch casing with a minimum penetration requirement of 15 inches using wireline."

**🤖 AI Agent:**
> The recommended gun system is the CP-15-W, which provides an estimated penetration of 16.2 inches and fits within the 7-inch casing.

---

**👤 You:**
> "Is a 500lb gun assembly safe to deploy via wireline if the limit is 450lbs?"

**🤖 AI Agent:**
> No, the deployment is not feasible as the gun weight exceeds the wireline limit.

---

**👤 You:**
> "What is the penetration depth for charge type 'X-200' in a formation with a hardness of 1.2?"

**🤖 AI Agent:**
> The effective penetration depth for the X-200 charge in this formation is 14.4 inches.


## ❓ FAQ

**Q: How does the engine handle different conveyance methods?**
The engine uses `calculate_system_capacity` to verify if a gun weight is safe for either wireline or TCP (Tubing Conveyed Perforating) based on specified weight limits.

**Q: Can I predict penetration depth for specific rock types?**
Yes, by using `evaluate_penetration_capability`, you can adjust the base performance of a charge using a formation hardness multiplier to predict effective depth.

**Q: What information is needed to recommend a gun system?**
To use `select_optimal_system`, you need the casing internal diameter, the minimum required penetration depth, and the intended conveyance method.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/perforating-gun-selection-engine](https://vinkius.com/en/ai-agent-connect/perforating-gun-selection-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perforating Gun Selection Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perforating-gun-selection-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perforating Gun Selection Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perforating-gun-selection-engine": {
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
