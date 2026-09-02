# Vapor-Liquid Equilibrium Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vapor-liquid-equilibrium-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate bubble points, dew points, and phase equilibrium properties for chemical mixtures.

## Description
This MCP server provides specialized thermodynamic tools for chemical process engineering. It allows AI agents to calculate critical phase equilibrium properties such as bubble points and dew points using various thermodynamic models. Users can determine equilibrium compositions and K-values for complex mixtures, and check for the existence of azeotropes. The engine supports ideal models, activity models, and Equations of State (EOS) to handle both ideal and non-ideal chemical behaviors.


## Available Tools (4)
- **calculate_dew_point**: Determines the conditions required for the first drop of liquid to form from a vapor mixture
- **calculate_bubble_point**: Determines the conditions required for the first bubble of vapor to form from a liquid mixture
- **check_azeotrope_existence**: Identifies if a mixture of specific components can form an azeotrope under specific conditions
- **get_equilibrium_properties**: Calculates K-values and phase compositions at a fixed temperature and pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vapor-Liquid Equilibrium Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the bubble point of a mixture of Benzene and Toluene at 1 atm using an ideal model? Composition: Benzene 0.4, Toluene 0.6"

**🤖 AI Agent:**
> The bubble point temperature for the Benzene-Toluene mixture at 1 atm is 85.4°C.

---

**👤 You:**
> "Check if Ethanol and Water can form an azeotrope using an activity model."

**🤖 AI Agent:**
> Yes, Ethanol and Water can form an azeotrope.

---

**👤 You:**
> "Calculate the equilibrium properties for a mixture of Methanol and Acetone at 350K and 2 atm using the eos model. Composition: Methanol 0.5, Acetone 0.5"

**🤖 AI Agent:**
> At 350K and 2 atm, the K-values are Methanol: 1.25 and Acetone: 0.85. The system is in the two-phase region.


## ❓ FAQ

**Q: What thermodynamic models are supported?**
The engine supports Ideal models, Activity models (like NRTL), and Equations of State (EOS) for non-ideal behavior.

**Q: How do I check if a mixture will form an azeotrope?**
You can use the `check_azeotrope_existence` tool to identify if specific components can form an azeotrope under given conditions.

**Q: Can I calculate the bubble point of a mixture?**
Yes, the `calculate_bubble_point` tool determines the temperature or pressure required for the first bubble of vapor to form from a liquid mixture.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vapor-liquid-equilibrium-engine](https://vinkius.com/ai-agent-connect/vapor-liquid-equilibrium-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vapor-Liquid Equilibrium Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vapor-liquid-equilibrium-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vapor-Liquid Equilibrium Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vapor-liquid-equilibrium-engine": {
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
