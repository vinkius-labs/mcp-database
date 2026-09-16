# Surfboard Blank Selection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surfboard-blank-selection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-tools](../categories/design-tools.md)

Select optimal foam blanks for surfboard shaping based on dimensions and buoyancy.

## Description
This MCP server provides precision decision-support for surfboard shapers. It connects AI agents to a specialized database of foam blanks, allowing for automated selection based on target geometry and buoyancy needs. Use `find_suitable_blanks` to see available stock, `calculate_cut_plan` for precise trimming measurements, `evaluate_buoyancy_fit` to check density compatibility, and `optimize_blank_selection` to minimize foam waste. It is designed to bridge the gap between design intent and raw material availability.


## Available Tools (4)
- **evaluate_buoyancy_fit**: Determine if a specific blank density and volume will result in desired buoyancy
- **calculate_cut_plan**: Provide specific trimming instructions for a selected blank
- **find_suitable_blanks**: Identify all available foam blanks that are large enough for the target dimensions
- **optimize_blank_selection**: Find the single best blank that minimizes waste while meeting all requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surfboard Blank Selection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all foam blanks suitable for a surfboard that is 180cm long, 50cm wide, and 6cm thick."

**🤖 AI Agent:**
> I found 3 suitable blanks: High-Performance Pro-X (185x52x7), Standard Lite (190x55x8), and Budget Heavy (200x60x10).

---

**👤 You:**
> "What are the trimming instructions for the High-Performance Pro-X blank to reach 180cm length, 50cm width, and 6cm thickness?"

**🤖 AI Agent:**
> To reach your target dimensions using the High-Performance Pro-X, you need to trim 5cm from the length, 2cm from the width, and 1cm from the thickness. This results in a waste percentage of 12.4%.

---

**👤 You:**
> "Which blank is best for a 175x45x5cm board with 35L volume and a preferred density of 0.04?"

**🤖 AI Agent:**
> The best choice is the Standard Lite blank, as it provides the closest density match while minimizing total foam waste.


## ❓ FAQ

**Q: How do I find a blank that fits my surfboard design?**
You can use the `find_suitable_blanks` tool by providing your target length, width, and thickness. The tool will return a list of all available foam blocks that meet or exceed those dimensions.

**Q: Can this tool help me reduce foam waste?**
Yes, the `optimize_blank_selection` tool is specifically designed to find the best blank that minimizes the volume difference between the raw foam and your target shape.

**Q: How do I know if the blank will provide enough buoyancy?**
Use the `evaluate_buoyancy_fit` tool. By providing the blank name and your target volume, the tool calculates a buoyancy score to ensure the density and volume match your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surfboard-blank-selection](https://vinkius.com/en/ai-agent-connect/surfboard-blank-selection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surfboard Blank Selection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surfboard-blank-selection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surfboard Blank Selection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surfboard-blank-selection": {
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
