# Thickener Sizing & Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/thickener-sizing-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate thickener diameter, depth, and overflow clarity using Coe-Clevenger or Talmage-Fitch models.

## Description
This MCP server provides essential engineering calculations for sizing tailings and concentrate thickeners. It allows AI agents to determine the minimum required diameter using `calculate_required_diameter`, calculate necessary vessel height with `calculate_required_depth`, and estimate liquid quality via `predict_overflow_clarity`. Additionally, users can use `optimize_flocculant_dosage` to find the ideal chemical balance between vessel size and operational costs.


## Available Tools (4)
- **optimize_flocculant_dosage**: Suggests the optimal chemical dosage to minimize diameter
- **calculate_required_depth**: Calculates the necessary height of the thickener
- **calculate_required_diameter**: Determines the minimum diameter required for a thickener
- **predict_overflow_clarity**: Estimates the quality of the liquid exiting the top


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thickener Sizing & Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What diameter do I need for a thickener with 15% feed solids, 60% target underflow density, and a settling velocity of 0.5 m/h using the Coe-Clevenger method?"

**🤖 AI Agent:**
> The required thickener diameter is 12.5 meters with a calculated surface area of 122.7 square meters.

---

**👤 You:**
> "How clear will the overflow be if I use a 10m diameter thickener with a settling velocity of 0.4 m/h and 10% feed solids?"

**🤖 AI Agent:**
> The predicted suspended solids concentration is 0.02% with a high clarity score.

---

**👤 You:**
> "Calculate the total depth needed for a 15m diameter thickener with a 50% target underflow density, a solids loading rate of 2.0 kg/m²s, and a residence time requirement of 3600 seconds."

**🤖 AI Agent:**
> The total required depth is 8.4 meters, consisting of a 5.2m settling zone and a 3.2m compression zone.


## ❓ FAQ

**Q: Which settling models are supported?**
The server supports both the Coe-Clevenger and Talmage-Fitch methods for calculating required diameter.

**Q: Can I optimize chemical usage?**
Yes, you can use the `optimize_flocculant_dosage` tool to find the best balance between diameter reduction and cost.

**Q: Does this tool account for flocculant impact?**
Yes, flocculant dosage is a parameter in diameter and clarity calculations, as it directly affects settling velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/thickener-sizing-design](https://vinkius.com/ai-agent-connect/thickener-sizing-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thickener Sizing & Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thickener-sizing-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thickener Sizing & Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thickener-sizing-design": {
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
