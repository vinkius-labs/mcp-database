# Acid Treatment Volume Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/acid-treatment-volume-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates acid volume, injection rates, and skin reduction for matrix acidizing.

## Description
This MCP server provides specialized tools for matrix acidizing design. It allows AI agents to calculate the required acid volume using `get_treatment_volume`, determine optimal flow rates with `calculate_injection_parameters`, estimate productivity improvements via `predict_skin_reduction`, and assess chemical risks using `evaluate_reaction_impact`.


## Available Tools (4)
- **calculate_injection_parameters**: Determines the appropriate flow rate to maintain control over the acid front
- **evaluate_reaction_impact**: Analyzes the potential for secondary damage from reaction products
- **get_treatment_volume**: Determines the total volume of acid required to treat the damaged zone
- **predict_skin_reduction**: Estimates the improvement in well productivity after the acid treatment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acid Treatment Volume Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the acid volume needed for a carbonate formation with a 2ft damage radius and 0.2 porosity using HCl_15."

**🤖 AI Agent:**
> The total volume required for the treatment is 15.7 cubic feet with an estimated spending rate of 0.05 units per minute.

---

**👤 You:**
> "What is the expected skin reduction if I treat a damage radius of 1.5ft with an initial skin of 5.0 using HCl_15?"

**🤖 AI Agent:**
> The final skin is estimated to be 1.2, resulting in a skin reduction of 76% with a high effectiveness score.

---

**👤 You:**
> "Determine the injection rate for 50 cubic feet of acid to be injected over 4 hours in a sandstone formation."

**🤖 AI Agent:**
> The required injection rate is 12.5 cubic feet per hour, with an estimated pressure of 1200 psi.


## ❓ FAQ

**Q: How do I calculate the required acid volume?**
You can use the `get_treatment_volume` tool by providing the damage radius, porosity, formation composition, and the acid system being used.

**Q: Can I estimate the improvement in well productivity?**
Yes, the `predict_skin_reduction` tool estimates the final skin factor and the effectiveness score of the treatment.

**Q: How is the injection rate determined?**
The `calculate_injection_parameters` tool determines the appropriate flow rate based on the total volume and the target injection duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/acid-treatment-volume-calculator](https://vinkius.com/ai-agent-connect/acid-treatment-volume-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acid Treatment Volume Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acid-treatment-volume-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acid Treatment Volume Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acid-treatment-volume-calculator": {
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
