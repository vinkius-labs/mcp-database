# Skin Factor Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/skin-factor-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Quantify wellbore damage and geometric skin from pressure buildup data.

## Description
This MCP server provides specialized analytical tools for reservoir engineers to quantify wellbore damage and geometric inefficiencies. Using pressure buildup and flow data, engineers can use `calculate_total_skin` to determine the overall skin factor. The toolset also allows for detailed analysis through `decompose_skin_components` to separate damage from geometric effects, and `analyze_perforation_effects` to evaluate partial penetration impacts. Additionally, `validate_well_test_consistency` ensures that provided pressure and flow data align with reservoir properties.


## Available Tools (4)
- **analyze_perforation_effects**: Specifically calculates the skin contribution caused by partial penetration and perforation geometry
- **calculate_total_skin**: Determines the overall skin factor from pressure buildup test data
- **decompose_skin_components**: Separates the total skin into damage and geometric components
- **validate_well_test_consistency**: Checks if the provided pressure and flow data are physically consistent with the reservoir properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skin Factor Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total skin for a well with permeability 50 mD, thickness 20m, viscosity 1 cP, flow rate 500 bpd, and these pressure readings: [{'time': 1, 'pressure': 100}, {'time': 2, 'pressure': 110}, {'time': 3, 'pressure': 120}]."

**🤖 AI Agent:**
> The total skin factor is 5.2.

---

**👤 You:**
> "Decompose a total skin of 10.0 with a penetration ratio of 0.8 and perforation efficiency of 0.9."

**🤖 AI Agent:**
> The damage skin is 7.2 and the geometric skin is 2.8.

---

**👤 You:**
> "Analyze perforation effects for a well with radius 0.1m, perforated length 5m, and reservoir thickness 10m."

**🤖 AI Agent:**
> The partial penetration skin is 1.5 and the perforation skin is 0.5.


## ❓ FAQ

**Q: What is the purpose of the `calculate_total_skin` tool?**
The `calculate_total_skin` tool determines the overall skin factor by analyzing the relationship between the pressure buildup slope and the flow rate.

**Q: Can I separate damage skin from geometric skin?**
Yes, you can use `decompose_skin_components` to separate the total skin into its damage and geometric components based on penetration ratio and efficiency.

**Q: How do I check if my well test data is valid?**
You can use the `validate_well_test_consistency` tool to check if the provided pressure and flow data are physically consistent with the reservoir properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/skin-factor-calculator](https://vinkius.com/en/ai-agent-connect/skin-factor-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skin Factor Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skin-factor-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skin Factor Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skin-factor-calculator": {
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
