# Sand Control Screen Selection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sand-control-screen-selection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Select optimal sand control screens based on formation grain size and well conditions.

## Description
This MCP server provides specialized engineering tools to select the most effective sand control screens for wellbore stability. By analyzing formation grain size distribution (GSD) and wellbore fluid dynamics, users can determine the ideal screen type, such as wire-wrap or premium screens, and calculate precise gauge openings. The tools evaluate operational risks like plugging and erosion to ensure long-term sand retention and well integrity.


## Available Tools (4)
- **calculate_opening_size**: Calculates the ideal slot or gauge opening to ensure sand retention while balancing flow capacity
- **evaluate_operational_risk**: Assesses the risks of screen failure due to plugging or erosion based on wellbore fluid dynamics and grain characteristics
- **generate_selection_summary**: Consolidates all engineering inputs into a final selection report for the user
- **get_screen_type**: Determines the most appropriate category of screen based on the selected sand control method and reservoir stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sand Control Screen Selection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What screen type should I use for a standalone method in a low stability formation?"

**🤖 AI Agent:**
> For a standalone method in a low stability formation, a premium screen is recommended to ensure high sand retention and erosion resistance.

---

**👤 You:**
> "Calculate the opening size for a formation with a d50 of 0.2mm and d10 of 0.05mm using a gravel pack method."

**🤖 AI Agent:**
> The recommended gauge opening for these parameters is 0.15mm, providing a sufficient retention safety factor for the gravel pack.

---

**👤 You:**
> "What are the risks if I have a flow velocity of 5.0 m/s and high particle concentration with a mesh screen?"

**🤖 AI Agent:**
> With a flow velocity of 5.0 m/s and high particle concentration, a mesh screen carries a high risk of erosion and a medium risk of plugging.


## ❓ FAQ

**Q: How do I determine the best screen type for my well?**
You can use the `get_screen_type` tool by providing the sand control method and the qualitative stability of the formation.

**Q: Can this tool help prevent wellbore plugging?**
Yes, by using `calculate_opening_size` and `evaluate_operational_risk`, you can assess the risk of plugging and select an aperture that balances sand retention with flow capacity.

**Q: What inputs are required for the risk assessment?**
To use `evaluate_operational_risk`, you need to provide the expected fluid flow velocity, the particle concentration, and the selected screen type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sand-control-screen-selection](https://vinkius.com/ai-agent-connect/sand-control-screen-selection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sand Control Screen Selection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sand-control-screen-selection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sand Control Screen Selection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sand-control-screen-selection": {
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
