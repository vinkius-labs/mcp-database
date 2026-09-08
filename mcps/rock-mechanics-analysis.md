# Rock Mechanics Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rock-mechanics-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze rock mass stability and determine mining support requirements.

## Description
This MCP server provides specialized tools for geotechnical engineering and mine design. It allows AI agents to calculate the Rock Mass Rating (RMR) using `analyze_rmr`, evaluate tunnel quality via the Q-system with `analyze_q_system`, determine necessary engineering measures through `estimate_support_requirements`, and assess excavation safety using `evaluate_stability`.


## Available Tools (4)
- **analyze_q_system**: Calculates the Q-index to evaluate rock mass quality for tunnel design
- **analyze_rmr**: Calculates the Rock Mass Rating (RMR) and provides a basic rock mass description
- **estimate_support_requirements**: Determines the type and density of support needed for an excavation
- **evaluate_stability**: Assesses the likelihood of failure in an excavation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rock Mechanics Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RMR for a rock with 60% RQD, 20mm joint spacing, smooth joints, and dry conditions, with an unconfined compressive strength of 50 MPa."

**🤖 AI Agent:**
> The calculated Rock Mass Rating (RMR) is 55, which classifies the rock as Class III (Fair Rock).

---

**👤 You:**
> "What support is needed for a 5-meter wide excavation in rock with a Q-index of 4.0 and a stress level of 10 MPa?"

**🤖 AI Agent:**
> The required support is mediumSupport, consisting of standard bolting and thin shotcrete layers.

---

**👤 You:**
> "Evaluate the stability of an excavation with a rock mass quality of 45 and significant structural discontinuities under 5 MPa of stress."

**🤖 AI Agent:**
> The stability rating is Moderate with a High failure risk due to the presence of structural discontinuities.


## ❓ FAQ

**Q: What classification systems are supported?**
The server supports the Rock Mass Rating (RMR) system and the Q-system for rock mass characterization.

**Q: Can I estimate support needs for a tunnel?**
Yes, you can use `estimate_support_requirements` to determine the type and density of support needed based on rock quality and excavation span.

**Q: How is stability assessed?**
Stability is assessed using `evaluate_stability`, which considers the rock mass quality, structural discontinuities, and applied stress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rock-mechanics-analysis](https://vinkius.com/ai-agent-connect/rock-mechanics-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rock Mechanics Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rock-mechanics-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rock Mechanics Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rock-mechanics-analysis": {
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
