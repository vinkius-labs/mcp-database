# Pipeline Flow Assurance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-flow-assurance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze fluid transport risks, hydrate formation, and wax deposition in subsea and terrestrial pipelines.

## Description
This MCP server provides a suite of analytical tools to manage flow assurance risks in pipeline systems. It allows AI agents to evaluate the likelihood of gas hydrate formation using `get_hydrate_risk`, assess paraffin buildup with `get_wax_deposition_profile`, and monitor asphaltene stability via `get_asphaltene_stability`. Additionally, users can calculate available shutdown time with `get_operational_window` and receive specific chemical or mechanical recommendations through `get_mitigation_requirements` to ensure operational continuity.


## Available Tools (5)
- **get_asphaltene_stability**: Evaluates the stability of asphaltenes within the fluid
- **get_hydrate_risk**: Determines the likelihood of gas hydrate formation under current conditions
- **get_mitigation_requirements**: Recommends chemical or mechanical actions to prevent identified risks
- **get_operational_window**: Calculates the time available before critical risks manifest during a shutdown
- **get_wax_deposition_profile**: Assesses the risk of paraffin/wax buildup on the pipe walls


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Flow Assurance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the hydrate formation risk for a pipeline at 200 bar and 5 degrees Celsius with a seabed temperature of 4 degrees?"

**🤖 AI Agent:**
> The hydrate formation risk is high, with a dissociation temperature of 12.5 degrees Celsius and a safety margin of 7.5 degrees.

---

**👤 You:**
> "How much time do I have before the fluid reaches the wax appearance temperature during a shutdown?"

**🤖 AI Agent:**
> The available cooldown time is 14.2 hours before the critical temperature threshold is reached.

---

**👤 You:**
> "What mitigation is needed for high wax risk?"

**🤖 AI Agent:**
> For high wax risk, the recommended actions include pigging operations and thermal heating.


## ❓ FAQ

**Q: How can I check for hydrate formation risks?**
You can use the `get_hydrate_risk` tool by providing the fluid composition, operating pressure, operating temperature, and seabed temperature.

**Q: What is the purpose of the operational window tool?**
The `get_operational_window` tool calculates the cooldown time available before the fluid temperature reaches a critical threshold, such as the hydrate formation temperature.

**Q: Can this tool recommend mitigation strategies?**
Yes, by using `get_mitigation_requirements`, the tool provides chemical or mechanical recommendations based on the identified risk levels for hydrates, wax, and asphaltenes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-flow-assurance](https://vinkius.com/en/ai-agent-connect/pipeline-flow-assurance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Flow Assurance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-flow-assurance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Flow Assurance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-flow-assurance": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
