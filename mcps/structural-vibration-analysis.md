# Structural Vibration Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/structural-vibration-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze floor vibration serviceability and natural frequencies.

## Description
This MCP server provides tools to determine the serviceability of floor structures. It calculates the natural frequency of a slab using `calculate_natural_frequency` and determines peak acceleration with `calculate_vibration_acceleration`. Users can then use `evaluate_serviceability` to check if the floor meets the required limits for specific occupancy types like residential, office, or laboratory environments.


## Available Tools (4)
- **calculate_natural_frequency**: Determine the fundamental natural frequency of a floor slab
- **calculate_vibration_acceleration**: Calculate the peak acceleration produced by specific vibration sources
- **evaluate_serviceability**: Determine if a floor is acceptable for a specific use case
- **get_occupancy_limits**: Retrieve the maximum allowable acceleration limits for different floor uses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Structural Vibration Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the natural frequency of a floor with a 5m span, 200mm thickness, and 0.05 damping ratio?"

**🤖 AI Agent:**
> The natural frequency of the floor is 12.5 Hz.

---

**👤 You:**
> "Is a floor with 0.02 m/s² acceleration acceptable for an office?"

**🤖 AI Agent:**
> Yes, the floor is acceptable for office use.

---

**👤 You:**
> "What are the acceleration limits for a laboratory?"

**🤖 AI Agent:**
> The maximum allowable acceleration for a laboratory is 0.005 m/s².


## ❓ FAQ

**Q: How do I check if a floor is suitable for a laboratory?**
You can use `evaluate_serviceability` after calculating the peak acceleration to see if it meets the strict limits required for laboratory environments.

**Q: What is the purpose of the natural frequency tool?**
The `calculate_natural_frequency` tool determines the fundamental frequency of a floor slab based on its span, thickness, and damping ratio.

**Q: Can I check acceleration limits for residential use?**
Yes, you can use `get_occupancy_limits` to retrieve the maximum allowable acceleration for residential occupancy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/structural-vibration-analysis](https://vinkius.com/ai-agent-connect/structural-vibration-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Structural Vibration Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `structural-vibration-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Structural Vibration Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "structural-vibration-analysis": {
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
