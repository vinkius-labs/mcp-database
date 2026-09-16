# Wine Foam Control MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-foam-control)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Manage fermentation foam levels and prevent tank overflow.

## Description
This MCP server provides specialized calculation tools for winemakers to manage foam levels during fermentation. It helps prevent tank overflow by assessing foam-over risk, calculating antifoam dosing, validating headspace adequacy, and recommending safe tank filling limits based on grape variety profiles. Use `calculate_foam_risk` to assess danger levels or `get_antifoam_recommendation` to determine necessary chemical additions.


## Available Tools (4)
- **get_antifoam_recommendation**: Calculates the necessary amount of antifoam agent to stabilize the foam
- **calculate_foam_risk**: Determines the current likelihood of a foam-over event
- **check_headspace_adequacy**: Validates if the current tank setup is safe for the current fermentation stage
- **recommend_fill_limits**: Suggests maximum liquid levels for new batches to prevent future issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Foam Control** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the risk of foam-over with 500L headspace, a fermentation rate of 10, protein content of 5, and foam potential of 8?"

**🤖 AI Agent:**
> The risk level is High with an overflow probability of 0.75.

---

**👤 You:**
> "Is my 1000L tank safe if I have 600L of liquid and expect 300L of foam expansion?"

**🤖 AI Agent:**
> Yes, the headspace is adequate with a safety margin of 100L.

---

**👤 You:**
> "How much antifoam do I need for 50L of foam with a stability of 0.8 and a target stability of 0.4?"

**🤖 AI Agent:**
> You should add 25.0L of antifoam in repeated small increments.


## ❓ FAQ

**Q: How can I prevent my fermentation tank from overflowing?**
You can use the `check_headspace_adequacy` tool to verify if your current tank setup is safe for the current fermentation stage.

**Q: How much antifoam should I add to my tank?**
The `get_antifoam_recommendation` tool calculates the exact dosage needed based on foam volume and stability.

**Q: Can I set filling limits for different grape varieties?**
Yes, the `recommend_fill_limits` tool suggests maximum liquid levels by accounting for the specific grape variety profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-foam-control](https://vinkius.com/en/ai-agent-connect/wine-foam-control)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Foam Control** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-foam-control` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Foam Control** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-foam-control": {
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
