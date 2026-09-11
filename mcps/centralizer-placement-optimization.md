# Centralizer Placement Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/centralizer-placement-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize centralizer spacing and count for effective wellbore cementing.

## Description
This MCP server provides technical decision support for optimizing centralizer placement in wellbores. It helps ensure effective primary cement jobs by calculating optimal spacing and quantity of centralizers based on hole deviation, casing size, and standoff requirements. Users can use `calculate_spacing_and_count` to determine the exact number of units needed, `evaluate_centralizer_compatibility` to assess deployment risks, `compare_strategies` to weigh bow-spring against rigid options, and `get_standoff_limits` to understand geometric boundaries.


## Available Tools (4)
- **compare_strategies**: Provides a side-by-side comparison of using bow-spring versus rigid centralizers for a specific well scenario
- **evaluate_compatibility**: Assesses whether a specific centralizer type is physically capable of being deployed in the given hole geometry
- **get_limits**: Queries the maximum and minimum theoretical standoff limits for a given casing/hole combination
- **calculate_spacing_and_count**: Determines the optimal distance between centralizers and the total quantity needed to maintain required standoff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Centralizer Placement Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the centralizer spacing for a 12-inch hole with 8.5-inch casing at a 30-degree deviation, requiring 70% standoff over 500 feet using rigid centralizers."

**🤖 AI Agent:**
> For a 12-inch hole and 8.5-inch casing at 30 degrees, the required spacing is 45 feet, requiring a total of 12 rigid centralizers to maintain a 70% standoff.

---

**👤 You:**
> "Is a rigid centralizer suitable for a 9-inch hole with 7-inch casing and 45-degree deviation?"

**🤖 AI Agent:**
> The deployment risk for rigid centralizers in this scenario is high due to the 45-degree deviation and limited clearance.

---

**👤 You:**
> "What are the theoretical standoff limits for an 8.5-inch hole and 5.5-inch casing?"

**🤖 AI Agent:**
> The maximum theoretical standoff is 0.85 and the minimum theoretical standoff is 0.00.


## ❓ FAQ

**Q: How do I determine the number of centralizers needed?**
You can use the `calculate_spacing_and_count` tool. By providing the hole diameter, casing diameter, deviation angle, target standoff, and interval length, the tool returns the total count and the required spacing distance.

**Q: Can I compare bow-spring and rigid centralizers?**
Yes, the `compare_strategies` tool provides a side-by-side comparison of both bow-spring and rigid options for your specific well scenario.

**Q: How is deployment risk assessed?**
The `evaluate_centralizer_compatibility` tool assesses deployment risk by analyzing the hole geometry and the chosen centralizer type, returning a risk level from low to high.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/centralizer-placement-optimization](https://vinkius.com/en/ai-agent-connect/centralizer-placement-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Centralizer Placement Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `centralizer-placement-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Centralizer Placement Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "centralizer-placement-optimization": {
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
