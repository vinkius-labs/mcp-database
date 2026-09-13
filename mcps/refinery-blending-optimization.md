# Refinery Blending Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-blending-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimizes refinery product blending using linear programming to maximize margins and ensure compliance.

## Description
This MCP server provides advanced optimization tools for refinery operations. It allows AI agents to manage component inventories, calculate precise blend recipes that account for nonlinear chemical properties, and solve global allocation problems to maximize refinery margins. By using `get_available_streams`, agents can monitor real-time inventory. The `calculate_blend_recipe` tool generates optimal component ratios, while `optimize_allocation` distributes limited streams across multiple product demands. Finally, `validate_product_compliance` ensures every blend meets strict regulatory and quality standards.


## Available Tools (4)
- **calculate_blend_recipe**: Determine the optimal volume of each component needed for a target product
- **get_available_streams**: Retrieve the current inventory of all available component streams
- **optimize_allocation**: Distribute available component streams across multiple product demands to maximize value
- **validate_product_compliance**: Verify if a specific blend recipe meets all legal and technical specifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Blending Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What component streams are currently available in the inventory?"

**🤖 AI Agent:**
> The current inventory includes Naphtha (5000L), Aromatics (2500L), and Alkylate (1200L).

---

**👤 You:**
> "Calculate a recipe for 1000 units of product 'HighOctane_01'."

**🤖 AI Agent:**
> To produce 1000 units of HighOctane_01, you need 600 units of Aromatics (60%) and 400 units of Naphtha (40%).

---

**👤 You:**
> "Is the blend of 50% Naphtha and 50% Aromatics compliant for product 'Standard_Fuel'?"

**🤖 AI Agent:**
> Yes, the blend is compliant with all regulatory and technical specifications for Standard_Fuel.


## ❓ FAQ

**Q: How does the tool handle nonlinear blending properties?**
The `calculate_blend_recipe` tool uses a specialized mathematical model to account for nonlinearities in properties like octane rating and vapor pressure, ensuring the resulting blend is realistic.

**Q: Can I use this to manage multiple product demands at once?**
Yes, the `optimize_allocation` tool is designed to solve the global optimization problem, distributing available component streams across various product demands to maximize total value.

**Q: How do I ensure my blends meet environmental regulations?**
You can use the `validate_product_compliance` tool to verify that a specific recipe adheres to all technical and regulatory limits before production.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-blending-optimization](https://vinkius.com/en/ai-agent-connect/refinery-blending-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Blending Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-blending-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Blending Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-blending-optimization": {
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
