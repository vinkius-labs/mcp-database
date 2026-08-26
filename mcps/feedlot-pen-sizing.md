# Feedlot Pen Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/feedlot-pen-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise feedlot pen dimensions, infrastructure needs, and performance impacts.

## Description
This MCP server provides precision engineering tools for livestock management. It allows AI agents to determine physical footprints, calculate necessary feed bunk lengths and waterer counts, and predict how pen density and mud conditions will affect animal weight gain. Use `calculate_pen_dimensions` to establish the initial layout, `calculate_infrastructure_needs` for equipment requirements, `estimate_performance_impact` to assess health risks, and `validate_site_suitability` to ensure compliance with regional welfare standards.


## Available Tools (4)
- **calculate_infrastructure_needs**: Calculates the necessary lengths for feeding and watering equipment
- **calculate_pen_dimensions**: Determines the physical footprint and number of pens required for a specific herd
- **estimate_performance_impact**: Predicts how the chosen pen density will affect animal weight gain and health
- **validate_site_suitability**: Checks if a proposed pen design meets minimum regulatory and welfare standards for a specific region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feedlot Pen Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pen dimensions for 500 cattle weighing 450kg each, with a 50% utilization rate and a mud score of 3."

**🤖 AI Agent:**
> The total required area is 12,500 m², consisting of 2 pens, each with an individual area of 6,250 m².

---

**👤 You:**
> "How much feed bunk length do I need for a pen with 50 animals weighing 500kg each, where the pen area is 1000 m² and the perimeter is 130 m?"

**🤖 AI Agent:**
> The required feed bunk length is 65 meters, with 2 waterers and a mound area requirement of 150 m².

---

**👤 You:**
> "What is the expected weight gain impact for 100 animals in a 2000 m² pen with a mud score of 4?"

**🤖 AI Agent:**
> The density score is 0.05, resulting in a moderate weight gain impact and a medium stress risk level.


## ❓ FAQ

**Q: How does mud score affect pen sizing?**
A higher mud score increases the required area per animal to maintain health and prevent overcrowding in wet conditions.

**Q: Can I check if my design meets regional regulations?**
Yes, you can use the `validate_site_suitability` tool to check if a design meets specific regional welfare standards.

**Q: What infrastructure details are provided?**
The `calculate_infrastructure_needs` tool provides the required feed bunk length, the number of waterers needed, and the required mound area for dry resting spots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/feedlot-pen-sizing](https://vinkius.com/ai-agent-connect/feedlot-pen-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feedlot Pen Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feedlot-pen-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feedlot Pen Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feedlot-pen-sizing": {
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
