# Leaching Kinetics Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/leaching-kinetics-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Models metal leaching kinetics to determine rate constants, activation energy, and leach time predictions.

## Description
This MCP server provides specialized tools for modeling the kinetics of metal leaching for gold and base metals. By analyzing ore mineralogy and experimental recovery data, users can calculate critical kinetic parameters such as the rate constant and activation energy. The server also identifies whether a process is under diffusion or reaction control and can predict the time required to reach specific extraction targets. Use `get_kinetic_parameters` to derive constants from experimental data, `predict_leach_time` for extraction forecasting, `analyze_mineralogy_impact` to assess ore resistance, and `simulate_leach_profile` to generate theoretical recovery curves.


## Available Tools (4)
- **get_kinetic_parameters**: Calculates fundamental kinetic constants from experimental recovery data
- **predict_leach_time**: Estimates how long it will take to reach a target metal extraction level
- **simulate_leach_profile**: Generates a theoretical recovery curve over time for a given set of conditions
- **analyze_mineralogy_impact**: Evaluates how the specific mineral composition affects the expected leaching difficulty


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leaching Kinetics Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the kinetic parameters for this recovery data at 45 degrees Celsius: [{'time': 1, 'recovery': 0.1}, {'time': 2, 'recovery': 0.25}, {'time': 3, 'recovery': 0.4}]"

**🤖 AI Agent:**
> The calculated rate constant is 0.15, the activation energy is 42.5 kJ/mol, and the process is dominated by reaction control.

---

**👤 You:**
> "How long will it take to reach 85% recovery if the rate constant is 0.12 and activation energy is 35?"

**🤖 AI Agent:**
> The estimated time to reach 85% recovery is 12.4 hours with a confidence interval of 0.8 hours.

---

**👤 You:**
> "What is the impact of an ore containing 30% silicates on gold leaching?"

**🤖 AI Agent:**
> The difficulty score is 0.75 and the expected rate modifier is 0.82, indicating significant resistance due to the silicate matrix.


## ❓ FAQ

**Q: How do I calculate the rate constant from my experimental data?**
You can use the `get_kinetic_parameters` tool by providing your recovery data as a JSON array of time and recovery objects along with the temperature used.

**Q: Can this model predict how long a leach cycle will take?**
Yes, once you have the kinetic parameters, you can use `predict_leach_time` to estimate the duration needed to reach a specific target recovery level.

**Q: How does mineralogy affect the leaching results?**
The `analyze_mineralogy_impact` tool evaluates how the specific composition of your ore affects the difficulty and the expected rate of the leaching process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/leaching-kinetics-model](https://vinkius.com/en/ai-agent-connect/leaching-kinetics-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leaching Kinetics Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leaching-kinetics-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leaching Kinetics Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leaching-kinetics-model": {
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
