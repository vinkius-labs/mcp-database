# Mouse Sensitivity Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mouse-sensitivity-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert mouse sensitivity, eDPI, and cm/360 precisely between competitive games like CS2, Valorant, and Apex Legends.

## Description
Maintain consistent muscle memory across different gaming engines with this high-precision converter. This MCP server provides tools to calculate exact sensitivity transfers using engine yaw values, compute eDPI (Effective Dots Per An Inch), determine physical mouse movement in cm/360, and adjust for FOV scaling impacts. Whether you are moving from CS2 to Valorant or adjusting settings for Apex Legends, use `convert_sensitivity` to find your new setting, `calculate_edpi` for hardware standardization, `calculate_cm_per_360` for physical distance tracking, and `calculate_fov_scaling` to account for field of view changes.


## Available Tools (4)
- **calculate_cm_per_360**: Calculates cm/360 distance
- **calculate_edpi**: Calculates eDPI
- **calculate_fov_scaling**: Calculates FOV scaling impact
- **convert_sensitivity**: Converts sensitivity between games


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mouse Sensitivity Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert my CS2 sensitivity of 1.5 to Valorant."

**🤖 AI Agent:**
> Your target sensitivity in Valorant is 0.84375.

---

**👤 You:**
> "What is my eDPI if I use 800 DPI and 1.2 sensitivity?"

**🤖 AI Agent:**
> Your eDPI is 960.

---

**👤 You:**
> "How many cm/360 is it at 800 DPI and 1.0 sensitivity in CS2?"

**🤖 AI Agent:**
> The physical distance required for a 360-degree turn is approximately 34.45 cm.


## ❓ FAQ

**Q: How accurate are the sensitivity conversions?**
The conversions are highly precise as they use the exact engine yaw constants for games like CS2, Valorant, and Apex Legends to calculate the ratio between different input scales.

**Q: What is eDPI and why does it matter?**
eDPI (Effective Dots Per Inch) is your mouse DPI multiplied by your in-game sensitivity. It provides a standardized way to compare sensitivity across different hardware settings using `calculate_edpi`.

**Q: Can I calculate physical mouse movement distance?**
Yes, the `calculate_cm_per_360` tool calculates exactly how many centimeters your mouse must travel on your pad to complete a full 360-degree turn in a specific game.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mouse-sensitivity-converter](https://vinkius.com/mcp/mouse-sensitivity-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mouse Sensitivity Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mouse-sensitivity-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mouse Sensitivity Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mouse-sensitivity-converter": {
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
