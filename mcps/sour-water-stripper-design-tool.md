# Sour Water Stripper Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sour-water-stripper-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design and size Sour Water Stripper (SWS) units for acid gas removal.

## Description
This MCP server provides specialized engineering tools for designing Sour Water Stripper (SWS) units. It allows users to calculate column dimensions, steam requirements, and effluent quality for both single-stage and high-efficiency two-stage configurations. Use `get_single_stage_design` for standard sizing, `get_two_stage_design` for high-efficiency requirements, or `compare_designs` to evaluate the trade-offs between CAPEX and OPEX. You can also use `validate_effluent_compliance` to ensure your stripped water meets environmental limits.


## Available Tools (4)
- **get_two_stage_design**: Calculates the dimensions and requirements for a high-efficiency two-stage stripping configuration
- **validate_effluent_compliance**: Checks if a given stripped water quality meets the required environmental or process specifications
- **get_single_stage_design**: Calculates the dimensions and requirements for a standard single-stage stripping column
- **compare_designs**: Provides a side-by-side comparison of single-stage and two-stage configurations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sour Water Stripper Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a single-stage design for 100 m3/h of sour water with 50 ppm H2S and 100 ppm NH3, targeting 5 ppm H2S and 10 ppm NH3."

**🤖 AI Agent:**
> The single-stage design requires a column diameter of 1.2 meters and a height of 15 meters, with a steam flow rate of 12.5 m3/h to achieve the target quality.

---

**👤 You:**
> "Compare single-stage and two-stage designs for 50 m3/h water, 100 ppm H2S, 200 ppm NH3, targeting 2 ppm H2S and 5 ppm NH3."

**🤖 AI Agent:**
> The two-stage design is recommended for this high-ammonia load as it provides significantly better steam efficiency despite the higher initial capital cost.

---

**👤 You:**
> "Is a stripped water sample with 8 ppm H2S and 12 ppm NH3 compliant with limits of 10 ppm H2S and 15 ppm NH3?"

**🤖 AI Agent:**
> Yes, the water is compliant as both H2S and NH3 concentrations are below the specified limits.


## ❓ FAQ

**Q: When should I use a two-stage design?**
A two-stage design is recommended when dealing with high ammonia concentrations or when extremely strict effluent limits must be met, as it optimizes steam consumption and separation efficiency.

**Q: How do I check if my water meets environmental limits?**
You can use the `validate_effluent_compliance` tool by providing the actual H2S and NH3 concentrations alongside your target limits.

**Q: What inputs are required for the design tools?**
The tools require the water flow rate, the concentration of H2S and NH3 in the feed, and the target effluent concentrations for both gases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sour-water-stripper-design-tool](https://vinkius.com/en/ai-agent-connect/sour-water-stripper-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sour Water Stripper Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sour-water-stripper-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sour Water Stripper Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sour-water-stripper-design-tool": {
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
