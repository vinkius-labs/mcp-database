# Acetylene Plant Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/acetylene-plant-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing acetylene production facilities.

## Description
This MCP server provides specialized engineering tools for designing acetylene production plants. It allows users to use `design_reactor` to specify physical vessel requirements based on feedstock like natural gas or calcium carbide. Engineers can then use `calculate_purification_requirements` to plan downstream cleaning, `evaluate_safety_protocols` to ensure compliance with pressure limits, and `generate_plant_summary` to consolidate all technical data into a final report.


## Available Tools (4)
- **design_reactor**: Determines the physical specifications of the primary reaction vessel
- **evaluate_safety_protocols**: Generates a mandatory safety compliance profile for the specific plant design
- **generate_plant_summary**: Consolidates reactor, purification, and safety data into a high-level engineering overview
- **calculate_purification_requirements**: Defines the necessary downstream equipment to clean the raw acetylene produced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acetylene Plant Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a reactor for an acetylene plant using natural gas with a capacity of 5000 units."

**🤖 AI Agent:**
> The reactor design for natural gas at 5000 units capacity specifies a partial oxidation vessel with high-capacity thermal management systems.

---

**👤 You:**
> "What are the purification needs for a calcium carbide based process with 15% impurities?"

**🤖 AI Agent:**
> For a 15% impurity level using calcium carbide, the purification plan requires specific scrubbing and filtration stages to reach industrial purity standards.

---

**👤 You:**
> "Check the safety protocols for a reactor operating at 20 bar pressure."

**🤖 AI Agent:**
> At 20 bar, the safety profile mandates the use of flame arrestors and specific high-pressure storage guidelines to prevent decomposition.


## ❓ FAQ

**Q: What feedstocks can I use for reactor design?**
You can select either natural_gas or calcium_carbide when using the `design_reactor` tool.

**Q: How do I get a final engineering report?**
Use the `generate_plant_summary` tool by providing the outputs from the reactor, purification, and safety tools.

**Q: Does this tool handle safety compliance?**
Yes, the `evaluate_safety_protocols` tool generates mandatory safety profiles based on your reactor type and operating pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/acetylene-plant-design](https://vinkius.com/en/ai-agent-connect/acetylene-plant-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acetylene Plant Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acetylene-plant-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acetylene Plant Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acetylene-plant-design": {
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
