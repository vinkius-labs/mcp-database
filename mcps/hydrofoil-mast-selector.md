# Hydrofoil Mast Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hydrofoil-mast-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Recommends optimal mast length based on rider skill, water depth, and wave conditions.

## Description
This MCP server provides specialized tools for hydrofoil riders to optimize their equipment selection. By analyzing environmental factors like water depth and wave height alongside personal profiles such as skill level and riding style, it ensures safety and performance. Use `get_recommended_mast_length` to find the ideal setup, `evaluate_breach_risk` to prevent seabed contact, `analyze_maneuverability_profile` to understand handling, and `check_depth_suitability` to verify if a location is safe for your gear.


## Available Tools (4)
- **analyze_maneuverability_profile**: Describes the handling characteristics of a chosen mast length
- **check_depth_suitability**: Determines if a specific environment is even suitable for hydrofoiling with a given mast
- **evaluate_breach_risk**: Assesses the danger of hitting the seabed given a specific mast choice
- **get_recommended_mast_length**: Provides the primary recommendation for a specific rider and environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydrofoil Mast Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a beginner riding in 150cm of water with 30cm waves. I prefer cruising. What mast should I use?"

**🤖 AI Agent:**
> For your profile, a 65cm mast is recommended to provide sufficient stability and depth clearance.

---

**👤 You:**
> "Is a 90cm mast safe in 120cm of water with 40cm waves?"

**🤖 AI Agent:**
> No, using a 90cm mast in these conditions presents a high risk of breaching the seabed.

---

**👤 You:**
> "How will a 110cm mast affect my agility if I am an advanced rider?"

**🤖 AI Agent:**
> An advanced rider using a 110cm mast will experience high agility but lower stability compared to shorter masts.


## ❓ FAQ

**Q: How does wave height affect my mast choice?**
Higher waves increase the risk of hitting the seabed. You can use `evaluate_breach_risk` to check if your chosen mast length provides enough clearance during wave troughs.

**Q: Can I use this for racing or just cruising?**
The tool supports multiple riding styles including cruising, carving, and racing. Simply specify your style in `get_recommended_mast_length`.

**Q: What happens if I am a beginner?**
For beginners, the tool prioritizes stability and safety. You can use `analyze_maneuverability_profile` to see how a specific mast length affects your stability score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hydrofoil-mast-selector](https://vinkius.com/ai-agent-connect/hydrofoil-mast-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydrofoil Mast Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydrofoil-mast-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydrofoil Mast Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydrofoil-mast-selector": {
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
