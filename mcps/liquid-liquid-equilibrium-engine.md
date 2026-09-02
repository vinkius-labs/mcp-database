# Liquid-Liquid Equilibrium Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/liquid-liquid-equilibrium-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-computing](../categories/scientific-computing.md)

Calculates phase compositions, distribution coefficients, and tie lines for immiscible liquid systems.

## Description
This MCP server provides specialized thermodynamic tools for analyzing liquid-liquid equilibrium (LLE) in multi-component systems. It allows AI agents to determine phase compositions, calculate distribution coefficients, and generate tie lines for both Type I and Type II phase behaviors. Use `calculate_phase_compositions` to find component concentrations in separated phases, `calculate_distribution_coefficients` to find partitioning preferences, `generate_tie_lines` to map equilibrium relationships, and `analyze_phase_behavior` to identify miscibility gaps.


## Available Tools (4)
- **generate_tie_lines**: Identifies the equilibrium relationship between phases across a range of compositions for a specific temperature
- **analyze_phase_behavior**: Classifies the system behavior and identifies the presence of a miscibility gap
- **calculate_distribution_coefficients**: Calculates the partitioning preference of each component between the two phases
- **calculate_phase_compositions**: Determines the concentration of each component in each separated liquid phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liquid-Liquid Equilibrium Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the phase compositions for a mixture of Water (0.6) and Benzene (0.4) at 298K using the Standard Model?"

**🤖 AI Agent:**
> Phase 1 (Aqueous): Water 0.95, Benzene 0.05. Phase 2 (Organic): Water 0.02, Benzene 0.98.

---

**👤 You:**
> "Is this system a single phase at 350K with a composition of Water 0.5 and Benzene 0.5 using the Advanced Non-Ideal Model?"

**🤖 AI Agent:**
> No, the system exhibits a miscibility gap with a width of 0.15.

---

**👤 You:**
> "What is the distribution coefficient for Benzene between the two phases if Phase 1 is 0.1 Benzene and Phase 2 is 0.8 Benzene?"

**🤖 AI Agent:**
> The distribution coefficient for Benzene is 0.125.


## ❓ FAQ

**Q: What kind of phase behaviors can this engine model?**
The engine supports both Type I and Type II phase behavior models to account for different solubility patterns in immiscible systems.

**Q: How do I find the concentration of components in each phase?**
You can use the `calculate_phase_compositions` tool, providing the system composition, temperature, and the chosen thermodynamic model.

**Q: Can I calculate the partitioning preference of a component?**
Yes, use the `calculate_distribution_coefficients` tool by providing the compositions of the two phases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/liquid-liquid-equilibrium-engine](https://vinkius.com/ai-agent-connect/liquid-liquid-equilibrium-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liquid-Liquid Equilibrium Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liquid-liquid-equilibrium-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liquid-Liquid Equilibrium Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liquid-liquid-equilibrium-engine": {
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
