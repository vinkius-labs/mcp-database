# SCC Mix Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/scc-mix-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design high-performance Self-Compacting Concrete (SCC) mixes using EFNARC guidelines.

## Description
This MCP server provides specialized engineering tools for designing Self-Compacting Concrete (SCC) mixes. By following EFNARC principles, it calculates essential parameters like powder content, water/powder ratio, and admixture dosages. Use `calculate_mix_proportions` to generate a primary design, `verify_passing_ability` to ensure the mix can navigate reinforcement, and `check_segregation_stability` to prevent aggregate settlement. It is an essential bridge for engineers connecting AI agents to precise concrete mix optimization.


## Available Tools (4)
- **check_segregation_stability**: Assesses the risk of aggregate settlement and bleeding
- **calculate_mix_proportions**: Generates the primary SCC mix design based on target performance requirements
- **get_material_efficiency**: Provides a cost and efficiency overview of the design
- **verify_passing_ability**: Evaluates if the current mix design will successfully pass through reinforcement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SCC Mix Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an SCC mix design for 40 MPa strength with a 600mm flow diameter and 16mm aggregate."

**🤖 AI Agent:**
> The calculated mix design requires a powder content of 450 kg/m³, a water/powder ratio of 0.38, and a superplasticizer dosage of 1.2 kg/m³ to meet your 40 MPa target.

---

**👤 You:**
> "Will a mix with 400 kg/m³ powder and 20mm aggregate pass through reinforcement?"

**🤖 AI Agent:**
> The mix has a high blockage risk due to the large aggregate size relative to the powder content.

---

**👤 You:**
> "Check the stability of a mix with a 10s V-funnel time and 0.4 water/powder ratio."

**🤖 AI Agent:**
> The stability rating is high, with a low risk of segregation for this specific viscosity.


## ❓ FAQ

**Q: What standards does this tool follow?**
The tool follows the EFNARC guidelines for Self-Compacting Concrete (SCC) mix design.

**Q: How can I check if my mix will block in reinforcement?**
You can use the `verify_passing_ability` tool to evaluate if the powder content and aggregate size are sufficient for the target reinforcement.

**Q: Can I assess the risk of segregation?**
Yes, the `check_segregation_stability` tool assesses the risk of aggregate settlement based on V-funnel time and water/powder ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/scc-mix-designer](https://vinkius.com/ai-agent-connect/scc-mix-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SCC Mix Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scc-mix-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SCC Mix Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scc-mix-designer": {
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
