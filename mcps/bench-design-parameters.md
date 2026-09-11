# Bench Design Parameters MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bench-design-parameters)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal open-pit bench geometry including height, width, and inter-ramp angles.

## Description
This MCP server provides specialized tools for open-pit mine engineers to design safe and efficient bench geometries. Use `get_bench_height` to determine vertical limits based on rock stability, `calculate_bench_width` to ensure equipment clearance and rock catchment, and `estimate_inter_ramp_angle` to calculate overall pit wall slopes. The `validate_design_compliance` tool ensures all parameters meet safety standards for specific rock types and equipment dimensions.


## Available Tools (4)
- **calculate_bench_width**: Calculates the required horizontal bench width to ensure equipment safety and rock catchment
- **estimate_inter_ramp_angle**: Calculates the overall slope angle of the pit wall across multiple benches
- **get_bench_height**: Determines the optimal vertical height of a bench based on rock characteristics
- **validate_design_compliance**: Checks if a proposed set of design parameters meets standard safety and operational requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bench Design Parameters** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recommended bench height for Hard-Rock with large-scale equipment?"

**🤖 AI Agent:**
> The recommended bench height for Hard-Rock with large-scale equipment is 15 meters, with a maximum allowable height of 18 meters.

---

**👤 You:**
> "Calculate the required bench width for a 6-meter wide machine in Sedimentary rock."

**🤖 AI Agent:**
> The total required bench width is 12.5 meters, which includes a 9.0 meter working width and a 3.5 meter safety berm.

---

**👤 You:**
> "Is a design with 12m height and 10m width compliant for Weathered rock and a 5m wide machine?"

**🤖 AI Agent:**
> No, the design is non-compliant because the height exceeds the stability limits for Weathered rock.


## ❓ FAQ

**Q: How does rock type affect bench design?**
Rock type dictates stability. For example, using `get_bench_height` with 'Hard-Rock' will yield different results than 'Weathered' rock because harder rock supports steeper, higher benches.

**Q: Can I check if my design is safe?**
Yes, use the `validate_design_compliance` tool to check if your proposed height and width meet safety requirements for your specific equipment and rock type.

**Q: How is the inter-ramp angle calculated?**
The `estimate_inter_ramp_angle` tool calculates the overall slope by considering the bench height, total bench width, and the width of the catch bench.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bench-design-parameters](https://vinkius.com/en/ai-agent-connect/bench-design-parameters)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bench Design Parameters** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bench-design-parameters` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bench Design Parameters** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bench-design-parameters": {
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
