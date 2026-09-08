# Pillar Design Empirical MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pillar-design-empirical)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate rock pillar stability using empirical geotechnical formulas.

## Description
This MCP server provides specialized geotechnical tools to design stable rock pillars. By using the `pillar_stability_design` tool, engineers can calculate pillar strength, factor of safety, and stability status using the Obert-Duvall empirical formula. It accounts for pillar geometry, rock strength (UCS), and applied vertical stress to ensure underground stability.


## Available Tools (1)
- **pillar_stability_design**: Calculate rock pillar stability using the Obert-Duvall empirical formula


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pillar Design Empirical** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stability of a pillar with a width of 5m, height of 10m, UCS of 50MPa, and vertical stress of 15MPa."

**🤖 AI Agent:**
> The calculated pillar strength is 32.5 MPa, resulting in a factor of safety of 2.17, which indicates a stable pillar.

---

**👤 You:**
> "What is the stability for a 3m wide, 12m high pillar with 40MPa UCS and 20MPa stress?"

**🤖 AI Agent:**
> The pillar strength is 18.4 MPa, yielding a factor of safety of 0.92. This pillar is considered unstable.

---

**👤 You:**
> "Check stability for a pillar: width=8, height=4, ucs=60, verticalStress=25."

**🤖 AI Agent:**
> The pillar strength is 84.0 MPa, providing a factor of safety of 3.36, confirming high stability.


## ❓ FAQ

**Q: What formulas are used for calculations?**
The tool currently utilizes the Obert-Duvall empirical formula to determine pillar strength and stability.

**Q: What inputs are required for the stability tool?**
You need to provide the pillar width, height, the Unconfined Compressive Strength (UCS) of the rock, and the applied vertical stress.

**Q: How is the factor of safety interpreted?**
A factor of safety greater than one indicates the pillar is theoretically stable under the provided loading conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pillar-design-empirical](https://vinkius.com/ai-agent-connect/pillar-design-empirical)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pillar Design Empirical** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pillar-design-empirical` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pillar Design Empirical** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pillar-design-empirical": {
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
