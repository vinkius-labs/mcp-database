# McCabe-Thiele Method MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mccabe-thiele-method)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Perform binary distillation analysis including stage counts and feed locations.

## Description
This MCP server provides tools for binary distillation analysis using the McCabe-Thiele graphical method. It allows users to calculate the total number of theoretical stages, determine the optimal feed stage location, and find the minimum reflux ratio required for a specific separation. By using tools like `calculate_stages` and `get_minimum_reflux`, engineers can model distillation columns based on provided equilibrium data and feed conditions.


## Available Tools (4)
- **analyze_feed_impact**: Evaluates how changing the feed's thermal condition affects the number of stages and the feed location
- **validate_equilibrium_data**: Ensures the provided equilibrium data is mathematically sound and suitable for distillation calculations
- **calculate_stages**: Determines the total number of theoretical stages required to meet product purity specifications
- **get_minimum_reflux**: Calculates the minimum reflux ratio required to achieve the specified separation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **McCabe-Thiele Method** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stages for a benzene-toluene separation with feed composition 0.5, distillate 0.95, bottoms 0.05, reflux 2.0, and q-value 1.0 using this equilibrium data: [{"x":0, "y":0}, {"x":0.5, "y":0.6}, {"x":1, "y":1}]"

**🤖 AI Agent:**
> The distillation analysis requires 6 theoretical stages, with the feed stage located at stage 3.

---

**👤 You:**
> "What is the minimum reflux ratio for a separation with distillate 0.9 and bottoms 0.1 using the provided equilibrium data?"

**🤖 AI Agent:**
> The minimum reflux ratio required for this separation is 1.45.

---

**👤 You:**
> "Check if my equilibrium data is valid: [{"x":0, "y":0}, {"x":0.5, "y":0.4}, {"x":1, "y":1}]"

**🤖 AI Agent:**
> The equilibrium data is valid and monotonic.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can use `calculate_stages` to find the total theoretical stages and feed stage, or `get_minimum_reflux` to find the minimum reflux ratio for your separation.

**Q: How do I provide equilibrium data?**
Provide the equilibrium data as a JSON array of objects containing x and y coordinates representing the equilibrium curve.

**Q: Can I analyze the impact of different feed conditions?**
Yes, the `analyze_feed_impact` tool allows you to test a range of q-values to see how the thermal state of the feed affects the column design.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mccabe-thiele-method](https://vinkius.com/ai-agent-connect/mccabe-thiele-method)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **McCabe-Thiele Method** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mccabe-thiele-method` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **McCabe-Thiele Method** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mccabe-thiele-method": {
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
