# Gasoline Blend Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gasoline-blend-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate precise gasoline blend properties including RON, MON, AKI, and RVP.

## Description
This MCP server provides professional-grade tools for determining the chemical and performance properties of blended gasoline streams. It accounts for blending nonlinearity by applying interaction factors to RON, MON, and RVP. Use `calculate_blend_properties` to determine the final characteristics of a mixture, `check_specification_compliance` to verify if a blend meets regulatory limits, and `get_component_contribution` to analyze how specific components influence the final octane or volatility.


## Available Tools (4)
- **calculate_blend_properties**: Calculates the primary performance and volatility characteristics of a complete gasoline blend
- **get_component_contribution**: Evaluates the influence of a specific component on the final blend's volatility and octane
- **validate_blend_inputs**: Performs a preliminary check on the integrity of raw component data before expensive calculations
- **check_specification_compliance**: Determines if a calculated blend meets specific target requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gasoline Blend Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the properties for a blend of 70% Component A (RON 95, MON 90, RVP 7) and 30% Component B (RON 90, MON 85, RVP 12) with interaction factors of 0.5 for RON, 0.2 for MON, and -1.0 for RVP."

**🤖 AI Agent:**
> The calculated blend properties are: RON 92.5, MON 87.5, AKI 90.0, and RVP 8.1.

---

**👤 You:**
> "Is a blend with AKI 88, RON 92, MON 84, and RVP 9 compliant with limits of minAki: 87, maxRvp: 10?"

**🤖 AI Agent:**
> Yes, the blend is compliant with all specified limits.

---

**👤 You:**
> "How much does Component A contribute to the volatility of the blend?"

**🤖 AI Agent:**
> Component A contributes 0.7 to the total volatility contribution based on its fraction and RVP.


## ❓ FAQ

**Q: How does this tool handle octane nonlinearity?**
The `calculate_blend_properties` tool uses interaction factors to adjust the weighted average of RON and MON, accounting for molecular interactions that cause non-linear blending behavior.

**Q: Can I check if my blend meets regulatory standards?**
Yes, you can use the `check_specification_compliance` tool to compare your calculated blend properties against specific minimum and maximum limits for AKI, RON, MON, and RVP.

**Q: What inputs are required for a blend calculation?**
You need to provide a JSON array of component objects (containing name, fraction, RON, MON, and RVP) and a JSON object containing the interaction factors for RON, MON, and RVP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gasoline-blend-calculator](https://vinkius.com/en/ai-agent-connect/gasoline-blend-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gasoline Blend Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gasoline-blend-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gasoline Blend Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gasoline-blend-calculator": {
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
