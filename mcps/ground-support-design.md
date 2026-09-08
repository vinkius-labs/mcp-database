# Ground Support Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ground-support-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal rock bolt patterns and shotcrete thickness for underground excavations.

## Description
This MCP server provides specialized geotechnical engineering tools for underground excavation design. It allows AI agents to determine reinforcement requirements by calculating `calculate_bolt_pattern` for rock bolts and `calculate_shotcrete_requirement` for surface support. Users can also use `evaluate_stability_safety_factor` to verify if a proposed design meets safety standards based on rock mass quality and stress ratios. Finally, `get_design_summary` aggregates all technical specifications into a single work order.


## Available Tools (4)
- **get_design_summary**: Aggregates all design components into a single technical specification
- **calculate_bolt_pattern**: Determines the required type, length, and spacing of rock bolts
- **calculate_shotcrete_requirement**: Determines the necessary thickness of shotcrete to stabilize the excavation face
- **evaluate_stability_safety_factor**: Provides a high-level assessment of whether a proposed support design is sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ground Support Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the bolt pattern for a 5-meter wide excavation in 'Fair' rock with a stress ratio of 1.5."

**🤖 AI Agent:**
> The required reinforcement is a Resin Bolt with a length of 3.5 meters and a spacing of 1.2 meters.

---

**👤 You:**
> "What is the required shotcrete thickness for a 4-meter wide tunnel in 'Poor' rock with a stress ratio of 2.0?"

**🤖 AI Agent:**
> The required shotcrete thickness is 0.15 meters.

---

**👤 You:**
> "Is a design with 1.5m bolt spacing and 0.1m shotcrete safe for a 6m wide excavation in 'Good' rock with a stress ratio of 1.0?"

**🤖 AI Agent:**
> Yes, the design is stable with a safety factor of 1.8.


## ❓ FAQ

**Q: What inputs are required for bolt pattern calculation?**
To use `calculate_bolt_pattern`, you need to provide the rock mass quality, the stress ratio, and the excavation width in meters.

**Q: Can I verify if my design is safe?**
Yes, you can use the `evaluate_stability_safety_factor` tool to check if your proposed bolt spacing and shotcrete thickness provide an adequate safety factor for the given conditions.

**Q: How do I get a final technical specification?**
Once you have determined the bolt type, length, spacing, and shotcrete thickness, use `get_design_summary` to generate a complete technical specification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ground-support-design](https://vinkius.com/ai-agent-connect/ground-support-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ground Support Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ground-support-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ground Support Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ground-support-design": {
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
