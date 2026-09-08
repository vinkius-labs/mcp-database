# Shotcrete Mix Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/shotcrete-mix-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise shotcrete mix proportions, fiber dosages, and accelerator requirements.

## Description
This MCP server provides specialized engineering tools for designing shotcrete mixtures used in tunnel support, mining, and slope stabilization. It allows AI agents to calculate core material volumes using `calculate_mix_proportions`, determine reinforcement needs with `calculate_fiber_dosage`, and manage chemical additives via `calculate_accelerator_dosage`. Additionally, it helps account for material waste by using `estimate_rebound_loss` to adjust total volumes based on application methods like wet or dry mix.


## Available Tools (4)
- **calculate_accelerator_dosage**: Calculate the chemical accelerator requirement based on the application method and environmental factors
- **calculate_mix_proportions**: Determine core material volumes required for a specific shotcrete application
- **calculate_fiber_dosage**: Determine the amount of reinforcement fibers needed to meet ductility requirements
- **estimate_rebound_loss**: Calculate the extra material required to account for waste during spraying


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shotcrete Mix Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the mix proportions for a wet-mix shotcrete with a required strength of 35 MPa using sand and gravel."

**🤖 AI Agent:**
> The required mix proportions are: cement content: 420 kg/m³, water content: 185 kg/m³, aggregate content: 1550 kg/m³, for a total volume of 1.0 m³.

---

**👤 You:**
> "What is the fiber dosage for a synthetic fiber reinforcement with a target ductility of 5.0?"

**🤖 AI Agent:**
> The required fiber dosage is 5.5 kg/m³, resulting in a fiber volume fraction of 0.008.

---

**👤 You:**
> "Estimate the rebound loss for a dry-mix application using high-precision nozzle technique."

**🤖 AI Agent:**
> The estimated rebound is 12% with a volume multiplier of 1.136.


## ❓ FAQ

**Q: How do I calculate the cement and water requirements?**
Use the `calculate_mix_proportions` tool, providing the required strength in MPa, the application method (wet or dry), and the available aggregate types.

**Q: Can I account for material waste during spraying?**
Yes, use `estimate_rebound_loss` to determine the rebound percentage and volume multiplier based on your application method and nozzle technique.

**Q: How do I determine the amount of fiber reinforcement needed?**
You can use `calculate_fiber_dosage` by specifying the target ductility and the type of fiber, such as steel or synthetic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/shotcrete-mix-design-engineer](https://vinkius.com/ai-agent-connect/shotcrete-mix-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shotcrete Mix Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shotcrete-mix-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shotcrete Mix Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shotcrete-mix-design-engineer": {
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
