# Crown Pillar Thickness Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crown-pillar-thickness-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Determine required crown pillar thickness and stability safety for underground mining.

## Description
This MCP server provides specialized engineering tools to ensure the structural integrity of underground mining operations. It allows engineers to calculate the minimum thickness required for a crown pillar based on excavation span, depth, and rock quality. Users can validate existing pillar safety using a target factor of safety, adjust requirements for long-term weathering impacts, and generate specific monitoring protocols to prevent surface subsidence. By using `calculate_minimum_thickness` and `validate_stability_safety`, mining professionals can maintain surface stability and protect critical infrastructure.


## Available Tools (4)
- **assess_weathering_impact**: Adjust thickness or safety requirements based on expected geological degradation over time
- **calculate_minimum_thickness**: Determine the smallest allowable thickness for a crown pillar based on current excavation parameters
- **get_monitoring_protocol**: Determine required monitoring equipment and frequency based on the pillar's risk profile
- **validate_stability_safety**: Check if an existing or proposed pillar thickness meets the required safety margins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crown Pillar Thickness Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum thickness for a 10m span at 50m depth with a rock quality index of 70 and high surface constraints?"

**🤖 AI Agent:**
> The minimum required thickness for these parameters is 8.5 meters, with a calculated factor of safety of 1.6.

---

**👤 You:**
> "Is a 5m thick pillar safe for a 15m span at 30m depth if I need a factor of safety of 1.5 and rock quality is 80?"

**🤖 AI Agent:**
> No, the current thickness is insufficient. The calculated factor of safety is only 1.2, which is below your target of 1.5.

---

**👤 You:**
> "What monitoring is needed for a pillar with a factor of safety of 1.3 and low rock quality?"

**🤖 AI Agent:**
> Due to the low factor of safety and rock quality, high-frequency monitoring using real-time electronic sensors is required.


## ❓ FAQ

**Q: How do I calculate the minimum thickness needed for my excavation?**
You can use the `calculate_minimum_thickness` tool by providing the excavation span, depth, rock quality index, and the surface constraint level.

**Q: Can I check if my current pillar is safe?**
Yes, use the `validate_stability_safety` tool to compare your current thickness against a target factor of safety to determine if the pillar is safe.

**Q: How does weathering affect my calculations?**
The `assess_weathering_impact` tool allows you to adjust your thickness requirements to account for the predicted degradation of rock strength over a specific time horizon.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crown-pillar-thickness-calculator](https://vinkius.com/ai-agent-connect/crown-pillar-thickness-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crown Pillar Thickness Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crown-pillar-thickness-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crown Pillar Thickness Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crown-pillar-thickness-calculator": {
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
