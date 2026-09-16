# Surf Break Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-break-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Classifies surf break types and predicts wave quality based on bathymetry and swell conditions.

## Description
This MCP server provides specialized tools for oceanographers and surfers to analyze surf zones. By analyzing the seabed structure and incoming swell, you can use `identify_break_type` to determine if a location is a beach, reef, or point break. The server also allows for predicting wave performance via `evaluate_wave_quality`, finding the best water levels with `calculate_optimal_tide`, and checking swell angles using `analyze_swell_alignment`.


## Available Tools (4)
- **analyze_swell_alignment**: Checks if the current swell is hitting the break at the correct angle
- **calculate_optimal_tide**: Identifies the best water level for surfing at a specific location
- **evaluate_wave_quality**: Predicts how well a specific swell will perform at a given break
- **identify_break_type**: Determines the fundamental category of the surf break


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Break Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What kind of surf break is a sandy bottom with a 5-degree slope?"

**🤖 AI Agent:**
> The seabed structure indicates a beach break.

---

**👤 You:**
> "Will a 4ft swell with a 12s period be good at a reef break?"

**🤖 AI Agent:**
> The wave quality is expected to be Good with a Peeling shape and High consistency.

---

**👤 You:**
> "What is the best tide for a reef break with a steep slope?"

**🤖 AI Agent:**
> The optimal tide for this reef break is Mid Tide.


## ❓ FAQ

**Q: How do I determine the type of surf break?**
You can use the `identify_break_type` tool by providing the bathymetry profile and the slope steepness of the seabed.

**Q: Can I predict if the waves will be good for surfing?**
Yes, the `evaluate_wave_quality` tool predicts wave shape, consistency, and a quality rating based on swell height, period, and direction.

**Q: Does the tide affect the results?**
Yes, the `calculate_optimal_tide` tool helps identify the best water level for specific break types to ensure safety and wave quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-break-classifier](https://vinkius.com/en/ai-agent-connect/surf-break-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Break Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-break-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Break Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-break-classifier": {
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
