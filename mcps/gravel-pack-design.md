# Gravel Pack Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gravel-pack-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for sand control completions using Saucier's sizing criteria.

## Description
This MCP server provides specialized engineering calculations for sand control in oil and gas completions. It uses Saucier's criterion to determine the optimal gravel size based on formation sand properties. Users can calculate the required `design_screen_slots` to ensure gravel retention, estimate the `calculate_gravel_volume` needed for the wellbore, and use `select_completion_fluid` to recommend the best carrier fluid for the placement method. It is designed to ensure wellbore stability and prevent formation sand invasion.


## Available Tools (4)
- **calculate_gravel_volume**: Estimates the total volume of gravel required for the completion
- **calculate_optimal_gravel_size**: Determines the appropriate gravel size based on the formation sand properties
- **design_screen_slots**: Calculates the required slot width to ensure gravel retention
- **select_completion_fluid**: Recommends a carrier fluid based on the design parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gravel Pack Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal gravel size for a formation with a median sand diameter of 0.002 meters?"

**🤖 AI Agent:**
> The optimal gravel diameter is 0.012 meters using a standard Saucier multiplier.

---

**👤 You:**
> "How much gravel do I need for a 100m well with an inner diameter of 0.2m and outer diameter of 0.3m using open hole placement and a 1.2 excess factor?"

**🤖 AI Agent:**
> The total volume of gravel required is 1.131 cubic meters.

---

**👤 You:**
> "Recommend a carrier fluid for an open hole placement with high formation sensitivity and gravel density of 2650 kg/m3."

**🤖 AI Agent:**
> A low-viscosity water-based brine is recommended to minimize formation damage while maintaining stability.


## ❓ FAQ

**Q: How is the gravel size determined?**
The gravel size is determined using the `calculate_optimal_gravel_size` tool, which applies Saucier's criterion by multiplying the median sand diameter by a safety factor.

**Q: Can I calculate the required gravel volume?**
Yes, the `calculate_gravel_volume` tool estimates the total volume required based on wellbore dimensions, placement method, and an excess factor.

**Q: How do I ensure the gravel stays in the wellbore?**
You can use the `design_screen_slots` tool to calculate the appropriate slot width to prevent gravel from passing through the screen.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gravel-pack-design](https://vinkius.com/en/ai-agent-connect/gravel-pack-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gravel Pack Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gravel-pack-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gravel Pack Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gravel-pack-design": {
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
