# Concrete Torsion Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-torsion-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [structural-engineering](../categories/structural-engineering.md)

Design reinforced concrete members for torsion using ACI provisions.

## Description
This MCP server provides structural engineering tools to design reinforced concrete members subjected to torsional loads. It follows ACI provisions to manage the interaction between shear and torsion. Users can determine required reinforcement using `calculate_torsion_reinforcement`, evaluate remaining shear capacity with `evaluate_shear_capacity`, identify torsion types via `check_torsion_type`, and verify section adequacy with `validate_section_geometry` to prevent web crushing.


## Available Tools (4)
- **calculate_torsion_reinforcement**: Determines the required amount of closed stirrups and longitudinal steel for a given torsional load
- **check_torsion_type**: Analyzes if the provided loading scenario qualifies as equilibrium or compatibility torsion
- **evaluate_shear_capacity**: Calculates the remaining shear capacity of a member after accounting for the presence of torsion
- **validate_section_geometry**: Verifies if the concrete section dimensions are sufficient to prevent web crushing under the specified torsion and shear


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Torsion Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reinforcement needed for a 300x500mm section with 10 kNm torsion and 50 kN shear (concrete 30 MPa, steel 400 MPa, equilibrium)."

**🤖 AI Agent:**
> The required stirrup area is 125 mm² and the total longitudinal steel area is 210 mm².

---

**👤 You:**
> "Is a 200x200mm section adequate for 15 kNm torsion and 40 kN shear with 25 MPa concrete?"

**🤖 AI Agent:**
> No, the section geometry is inadequate and exceeds the crushing threshold.

---

**👤 You:**
> "What is the remaining shear capacity for a 400x400mm section with 5 kNm torsion and 100 kN shear?"

**🤖 AI Agent:**
> The available shear capacity is 145 kN with a utilization ratio of 0.68.


## ❓ FAQ

**Q: How does this tool handle equilibrium vs compatibility torsion?**
The `check_torsion_type` tool identifies the category. If the system is statically determinate, it is treated as Equilibrium torsion, requiring full reinforcement resistance.

**Q: Can I check if my concrete section is large enough?**
Yes, use `validate_section_geometry` to verify if the section dimensions prevent web crushing under the specified torsion and shear loads.

**Q: Does it account for combined shear and torsion effects?**
Yes, `evaluate_shear_capacity` applies ACI interaction equations to calculate the remaining shear capacity after accounting for torsional stress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-torsion-design](https://vinkius.com/ai-agent-connect/concrete-torsion-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Torsion Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-torsion-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Torsion Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-torsion-design": {
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
