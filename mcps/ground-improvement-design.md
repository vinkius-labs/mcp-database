# Ground Improvement Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ground-improvement-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Technical design for soil improvement methods including stone columns, vibro-compaction, and grouting.

## Description
This MCP server provides specialized geotechnical engineering tools to design ground improvement strategies. It allows engineers to calculate technical parameters for various methods such as `calculate_stone_column_design` for cohesive soils, `calculate_vibro_compaction_design` for granular soils, and `calculate_grouting_design` for injection-based improvements. You can also use `validate_improvement_feasibility` to determine the most appropriate method based on soil properties like cohesion, permeability, and bearing capacity requirements.


## Available Tools (4)
- **calculate_grouting_design**: Determines the injection parameters for cementitious or chemical grouting
- **calculate_stone_column_design**: Determines technical parameters for improving soft cohesive soils using stone columns
- **calculate_vibro_compaction_design**: Determines the design for densifying granular soils via vibration
- **validate_improvement_feasibility**: Provides a high-level check to see if a specific method is appropriate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ground Improvement Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is vibro-compaction suitable for a cohesive soil with a required bearing capacity of 200 kPa?"

**🤖 AI Agent:**
> No, vibro-compaction is intended for granular soils. For cohesive soils, stone columns or grouting would be more appropriate.

---

**👤 You:**
> "Calculate the design for stone columns in a soil with 30 kPa cohesion, 25 degree friction angle, and 100 kPa modulus, needing 250 kPa bearing capacity and 25 mm settlement limit with a 0.2 replacement ratio."

**🤖 AI Agent:**
> The stone column design requires an improvement depth of 8.5m and a column spacing of 1.8m to meet the target replacement ratio and bearing capacity requirements.

---

**👤 You:**
> "What are the injection parameters for grouting in soil with 1e-5 m/s permeability?"

**🤖 AI Agent:**
> The grouting design requires an injection spacing of 1.2m and a replacement ratio of 0.05 to achieve the required soil stiffness.


## ❓ FAQ

**Q: What soil types can I design for?**
The tools support both cohesive and granular soils. You can use `validate_improvement_feasibility` to check which method is best for your specific soil type.

**Q: How do I calculate stone column spacing?**
Use the `calculate_stone_column_design` tool. Provide the soil cohesion, friction angle, modulus, required bearing capacity, settlement limit, and your target replacement ratio.

**Q: Can I use this for vibro-compaction design?**
Yes, the `calculate_vibro_compaction_design` tool is specifically designed to determine parameters for densifying granular soils via vibration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ground-improvement-design](https://vinkius.com/ai-agent-connect/ground-improvement-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ground Improvement Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ground-improvement-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ground Improvement Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ground-improvement-design": {
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
