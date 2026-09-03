# Concrete Crack Width Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-crack-width-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate and verify concrete crack widths based on structural reinforcement and environmental exposure.

## Description
This MCP server provides precise tools for structural engineers to predict and validate concrete cracking. Use `calculate_crack_width` to determine physical crack width and spacing based on reinforcement stress, bar diameter, and concrete properties. You can use `get_exposure_limits` to find maximum allowable widths for specific environmental classes like XC1 or XS1, and `validate_crack_compliance` to check if your measured cracks meet safety standards. Additionally, `analyze_geometry_impact` helps evaluate how changing the concrete cover or bar diameter affects crack propagation.


## Available Tools (4)
- **calculate_crack_width**: Determines the physical width of a crack based on mechanical and geometric inputs
- **get_exposure_limits**: g., XC1, XS1, XF1) to get the allowable crack width limits.

Retrieves the maximum allowable crack width based on the environmental exposure class
- **validate_crack_compliance**: Checks if a specific set of crack parameters meets the limits of a specific exposure class
- **analyze_geometry_impact**: Evaluates how changes in cover or bar diameter affect the potential crack width


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Crack Width Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the crack width for a reinforcement stress of 250 MPa, bar diameter of 20 mm, cover of 40 mm, concrete strength of 35 MPa, and a strain gradient of 0.001."

**🤖 AI Agent:**
> The calculated crack width is 0.12 mm with a spacing of 150 mm, which is compliant with standard exposure limits.

---

**👤 You:**
> "What is the maximum allowable crack width for the XS1 exposure class?"

**🤖 AI Agent:**
> For the XS1 exposure class, the maximum allowable crack width is 0.20 mm.

---

**👤 You:**
> "If I increase the concrete cover from 30 mm to 50 mm, how will it affect the crack width?"

**🤖 AI Agent:**
> Increasing the concrete cover to 50 mm results in a 15% reduction in the predicted crack width.


## ❓ FAQ

**Q: How do I check if my crack width is safe?**
Use the `validate_crack_compliance` tool. Provide the measured crack width and the relevant environmental exposure class to see if it meets safety limits.

**Q: Can I simulate changes in reinforcement geometry?**
Yes, the `analyze_geometry_impact` tool allows you to test how modifying the bar diameter or concrete cover affects the resulting crack width.

**Q: What environmental classes are supported?**
The tool supports standard exposure classes such as XC1, XS1, and XF1 via the `get_exposure_limits` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-crack-width-analyzer](https://vinkius.com/ai-agent-connect/concrete-crack-width-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Crack Width Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-crack-width-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Crack Width Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-crack-width-analyzer": {
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
