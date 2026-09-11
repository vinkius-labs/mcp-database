# Surfboard Fin Configurator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surfboard-fin-configurator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal fin geometry and setup for any wave condition.

## Description
This MCP server provides precise hydrodynamic calculations to determine the best fin setup for your surfboard. By analyzing wave size, speed, and your riding style, you can use `calculate_fin_setup` to find the ideal fin size and configuration. You can also use `analyze_hydrodynamic_efficiency` to evaluate drag and lift, or `optimize_toe_in` to maximize grip during turns. It is a specialized tool for surfers looking to optimize their equipment performance.


## Available Tools (4)
- **analyze_hydrodynamic_efficiency**: Evaluates how much drag a specific fin configuration will produce under given conditions
- **calculate_fin_setup**: Provides the primary recommendation for fin dimensions and configuration based on environmental and board parameters
- **get_style_presets**: Retrieves a list of supported riding styles and their characteristic characteristics
- **optimize_toe_in**: Calculates the specific angle for side fins to maximize grip without sacrificing too much speed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surfboard Fin Configurator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What fin setup should I use for a 1.5m wave with a 200cm board if I ride in a performance style?"

**🤖 AI Agent:**
> For a 1.5m wave and a 200cm board with a performance style, the recommended setup is a 4.5cm Thruster configuration with a 2.5 degree toe-in angle.

---

**👤 You:**
> "How much drag will a 5cm quad fin produce in a 2m/s wave speed?"

**🤖 AI Agent:**
> The quad fin setup at 2m/s wave speed results in a drag coefficient of 0.045 and an efficiency rating of High.

---

**👤 You:**
> "What is the best toe-in angle for a big-wave setup?"

**🤖 AI Agent:**
> For big-wave conditions, the optimal toe-in angle is 4.0 degrees to ensure maximum grip.


## ❓ FAQ

**Q: How do I get a recommendation for my board?**
You can use the `calculate_fin_setup` tool by providing your wave size, wave speed, riding style, and board length.

**Q: Can I check the drag of a specific fin?**
Yes, the `analyze_hydrodynamic_efficiency` tool allows you to evaluate the drag coefficient and lift for different fin types and foils.

**Q: What riding styles are supported?**
The tool supports Performance, Cruiser, and Big Wave styles. You can see all details using `get_style_presets`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surfboard-fin-configurator](https://vinkius.com/en/ai-agent-connect/surfboard-fin-configurator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surfboard Fin Configurator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surfboard-fin-configurator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surfboard Fin Configurator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surfboard-fin-configurator": {
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
