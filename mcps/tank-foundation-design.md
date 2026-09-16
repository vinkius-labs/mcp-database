# Tank Foundation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tank-foundation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Engineering tool for determining tank foundation types, settlement, and bearing capacity.

## Description
This MCP server provides specialized geotechnical engineering tools for liquid storage tank design. It allows AI agents to determine the most suitable foundation configuration using `get_foundation_type`, predict vertical movement with `calculate_settlement`, verify soil stability via `verify_bearing_capacity`, and evaluate earthquake impact with `assess_seismic_risk`.


## Available Tools (4)
- **assess_seismic_risk**: Evaluates the impact of seismic activity on the tank foundation stability
- **calculate_settlement**: Predicts the total expected settlement of the tank under its operating weight
- **get_foundation_type**: Determines the most suitable foundation configuration based on tank and soil constraints
- **verify_bearing_capacity**: Checks if the soil can safely support the tank's total weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tank Foundation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What foundation type is best for a 20m diameter tank in a high seismic zone with clay soil?"

**🤖 AI Agent:**
> Based on the high seismic zone and clay soil, a pile foundation is recommended to ensure stability and mitigate settlement risks.

---

**👤 You:**
> "Check if the soil can support a tank with a 15m diameter and 10m height."

**🤖 AI Agent:**
> The soil capacity is sufficient with a factor of safety of 2.5, resulting in a 'Pass' status.

---

**👤 You:**
> "What is the expected settlement for this tank design?"

**🤖 AI Agent:**
> The total predicted settlement is 12mm, which is within the acceptable engineering limits.


## ❓ FAQ

**Q: How do I determine the best foundation type?**
You can use the `get_foundation_type` tool, which analyzes tank dimensions, soil bearing capacity, soil type, and seismic zone to recommend a ringwall, slab, or pile foundation.

**Q: Can this tool help with seismic stability?**
Yes, the `assess_seismic_risk` tool evaluates how seismic activity impacts foundation stability and provides required mitigation steps.

**Q: How is soil settlement calculated?**
The `calculate_settlement` tool predicts both immediate and consolidation settlement based on tank load, soil compressibility, and ground water depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tank-foundation-design](https://vinkius.com/en/ai-agent-connect/tank-foundation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tank Foundation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tank-foundation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tank Foundation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tank-foundation-design": {
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
