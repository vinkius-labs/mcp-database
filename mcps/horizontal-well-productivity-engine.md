# Horizontal Well Productivity Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/horizontal-well-productivity-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate horizontal well productivity, optimal length, and penetration effects.

## Description
This MCP server provides specialized reservoir engineering computations for horizontal well design. It allows AI agents to evaluate well performance using Joshi or Economides models. Key capabilities include using `calculate_horizontal_productivity` to compare horizontal performance against vertical baselines, `optimize_well_length` to find the point of diminishing returns, `analyze_penetration_effects` to assess losses from eccentricity, and `compare_well_types` for high-level design assessments.


## Available Tools (4)
- **analyze_penetration_effects**: Evaluates how much productivity is lost due to the well not being centered or covering the full thickness
- **calculate_horizontal_productivity**: Calculates the productivity index of a horizontal well and compares it to a vertical well
- **compare_well_types**: Provides a high-level summary comparison between a proposed horizontal well and a standard vertical well
- **optimize_well_length**: Determines the most efficient horizontal length for a specific reservoir configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Horizontal Well Productivity Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the productivity index for a horizontal well with 500m length, 20 mD vertical permeability, 100 mD horizontal permeability, 15m thickness, 10 anisotropy, 1000m depth, 7.5m position, and 50 psi drawdown."

**🤖 AI Agent:**
> The calculated productivity index is 12.45, with a vertical baseline PI of 2.10, resulting in an improvement factor of 5.93.

---

**👤 You:**
> "What is the optimal length for a reservoir with 30 mD vertical permeability, 150 mD horizontal permeability, 20m thickness, and 5 anisotropy if I want a target PI of 15?"

**🤖 AI Agent:**
> The optimal length to achieve a target PI of 15 is 850 meters, with an estimated efficiency loss of 0.04.

---

**👤 You:**
> "Evaluate the impact of a well positioned 2 meters from the top in a 10 meter thick reservoir with 15 mD vertical permeability and 100m length."

**🤖 AI Agent:**
> The penetration efficiency is 0.82, resulting in a loss factor of 0.82 applied to the total productivity.


## ❓ FAQ

**Q: What models are used for productivity calculations?**
The engine utilizes Joshi and Economides models to determine the productivity index and compare it to vertical well baselines.

**Q: How does eccentricity affect the results?**
You can use `analyze_penetration_effects` to see how the well position within the reservoir thickness impacts the overall productivity efficiency.

**Q: Can I find the most efficient well length?**
Yes, the `optimize_well_length` tool calculates the optimal length where incremental productivity gains begin to stabilize.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/horizontal-well-productivity-engine](https://vinkius.com/en/ai-agent-connect/horizontal-well-productivity-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Horizontal Well Productivity Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `horizontal-well-productivity-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Horizontal Well Productivity Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "horizontal-well-productivity-engine": {
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
