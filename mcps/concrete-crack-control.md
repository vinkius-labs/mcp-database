# Concrete Crack Control MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-crack-control)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design reinforcement spacing and ratios to prevent concrete cracking.

## Description
This MCP server provides structural engineering tools to manage concrete durability. It allows agents to calculate the maximum allowable bar spacing using `calculate_max_bar_spacing`, determine the necessary reinforcement ratio with `calculate_reinforcement_ratio`, and predict crack widths via `estimate_crack_width`. By accounting for exposure classes like MARINE_SEA_SPRAY or DEICING_SALTS, it ensures reinforcement designs meet strict durability requirements.


## Available Tools (4)
- **estimate_crack_width**: Predicts the actual width of a crack produced by a specific reinforcement configuration
- **get_exposure_constraints**: Retrieves the standard crack width limits and safety factors associated with a specific environmental exposure class
- **calculate_max_bar_spacing**: Determines the largest possible distance between reinforcement bars to satisfy a specific crack width constraint
- **calculate_reinforcement_ratio**: Calculates the minimum percentage of steel area required relative to the concrete area to prevent exceeding crack limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Crack Control** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum bar spacing for a 20mm bar with 30mm cover and 250MPa stress in a marine environment with a 0.3mm crack limit?"

**🤖 AI Agent:**
> The maximum allowable bar spacing for this configuration is 185.5 mm.

---

**👤 You:**
> "Calculate the reinforcement ratio for 15mm bars, 40mm cover, 300MPa stress, and a 0.2mm crack limit in a de-icing salt environment."

**🤖 AI Agent:**
> The required reinforcement ratio is 0.0125.

---

**👤 You:**
> "Estimate the crack width for 12mm bars spaced at 150mm with 35mm cover and 280MPa stress in an urban dry environment."

**🤖 AI Agent:**
> The estimated crack width is 0.14 mm.


## ❓ FAQ

**Q: How do I find the maximum distance between bars?**
Use the `calculate_max_bar_spacing` tool. You will need to provide the concrete cover, bar diameter, steel stress, crack width limit, and the exposure class.

**Q: Can I predict the crack width for a specific setup?**
Yes, the `estimate_crack_width` tool calculates the expected width based on your bar spacing, diameter, and environmental exposure.

**Q: What exposure classes are supported?**
Supported classes include URBAN_DRY, DEICING_SALTS, MARINE_SEA_SPRAY, and FREEZING_THAWING.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-crack-control](https://vinkius.com/ai-agent-connect/concrete-crack-control)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Crack Control** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-crack-control` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Crack Control** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-crack-control": {
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
