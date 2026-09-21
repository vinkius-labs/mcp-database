# Indoor Garden Layout Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/indoor-garden-layout-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Deterministic design engine for optimizing indoor and balcony garden layouts.

## Description
This MCP server provides a deterministic design engine to create optimized indoor or balcony garden layouts. It calculates plant placements based on space dimensions, plant footprints, and light zones while ensuring human access paths are maintained. Use `get_optimal_layout` to generate a primary design, `validate_layout_compliance` to check for biological or physical violations, `generate_alternative_layouts` for aesthetic variety, and `calculate_space_utilization` to analyze area efficiency.


## Available Tools (4)
- **calculate_space_utilization**: Analyzes how efficiently the available area is being used
- **generate_alternative_layouts**: Provides different arrangement options when the primary layout is constrained or for aesthetic variety
- **get_optimal_layout**: Generates a single best-fit layout based on provided dimensions and plant list
- **validate_layout_compliance**: Checks an existing layout against specific biological and physical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indoor Garden Layout Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a garden layout for a 2m x 2m balcony with two sun-loving plants."

**🤖 AI Agent:**
> The optimal layout places Plant A at (0.5, 0.5) and Plant B at (1.5, 1.5), covering 1.2 square meters with no clearance violations.

---

**👤 You:**
> "Is my layout valid if I place a shade plant in a high intensity light zone?"

**🤖 AI Agent:**
> No, the layout is invalid because the plant's light requirement is not met by the assigned zone.

---

**👤 You:**
> "What is the efficiency of a 10sqm space with 4sqm of plants?"

**🤖 AI Agent:**
> The utilization percentage is 40% with 6 square meters of wasted area.


## ❓ FAQ

**Q: How do I generate a new garden design?**
You can use the `get_optimal_layout` tool by providing your space dimensions, a list of plants, and the available light zones.

**Q: Can I check if my current layout is safe?**
Yes, use `validate_layout_compliance` to check for clearance violations or light requirement mismatches.

**Q: How can I see how much space I am wasting?**
The `calculate_space_utilization` tool provides the utilization percentage and the total wasted area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/indoor-garden-layout-planner](https://vinkius.com/en/ai-agent-connect/indoor-garden-layout-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Indoor Garden Layout Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `indoor-garden-layout-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Indoor Garden Layout Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indoor-garden-layout-planner": {
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
