# Fire Safety Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fire-safety-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [structural-design](../categories/structural-design.md)

Calculate mandatory fire safety infrastructure requirements, including maximum evacuation distance, minimum stair width, and extinguisher density based on local building codes.

## Description
**The Challenge of Life Safety Compliance**

A commercial or public structure's safety relies entirely on its ability to manage emergencies. Failing to meet fire code standards can result in catastrophic loss of life and property, making compliance a critical structural risk.

**How This System Works**
This MCP connector provides specialized tools that model regulatory requirements based on real-world building physics and local mandates. It connects AI agents directly to the calculation logic needed for safe design.

1. **Evacuation Path Compliance:** Use `calculate_max_walking_distance` with the total area, population load, and construction type to ensure all exit paths are within regulatory limits.
2. **Stairway Capacity:** Utilize `determine_min_stair_width` by feeding it the floor population count and standardized module size (e.g., 60cm) to determine the absolute minimum required stair width.
3. **Fire Suppression Density:** Specify extinguisher needs using `specify_extinguisher_requirement`. Provide the total usable area and the risk class code (A, B, or C) to get an accurate count and distribution of fire suppression equipment.

The resulting data provides a definitive compliance report, ensuring your design meets stringent US and local Brazilian Fire Department standards.


## Available Tools (3)
- **specify_extinguisher_requirement**: Returns distribution by type (A, B, C) and compliance notes for placement.

Determine required fire extinguisher quantity and type distribution by area and risk class
- **determine_min_stair_width**: Returns minimum required width, population ratio details, and safe design recommendation with safety buffer.

Calculate minimum stair width based on population load and module definition
- **calculate_max_walking_distance**: Returns compliance status and violation details.

Calculate maximum walking distance compliance for evacuation paths


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fire Safety Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The new office building has an area of 1500 sqm, a population load of 450 people, and is classified as 'Class B Office'. Check if the evacuation paths are compliant."

**🤖 AI Agent:**
> I will use `calculate_max_walking_distance` with (1500, 450, 'Class B Office'). The result confirms compliance, and the maximum allowed distance is 75 meters. No potential violations found.

---

**👤 You:**
> "We need to know the minimum stair width for a floor with 800 people, using a standard module of 60cm."

**🤖 AI Agent:**
> Running `determine_min_stair_width` with (800, 60) shows the minimum required width is 480 cm. The recommendation suggests using a 528 cm stair for enhanced safety.

---

**👤 You:**
> "For a warehouse space of 900 sqm with 'Medium Risk' classification, how many fire extinguishers are needed?"

**🤖 AI Agent:**
> I executed `specify_extinguisher_requirement` using (900, 'Medium Risk'). The total required is 12 extinguishers: 6 ABC Dry Chemical and 6 Type B Foam.


## ❓ FAQ

**Q: What inputs are needed to check for safe evacuation distances?**
To use the `calculate_max_walking_distance` tool, you must provide three inputs: the building's total gross usable floor area in square meters, the maximum calculated population load, and a string specifying the construction type. This ensures compliance with local zone regulations.

**Q: How does the system calculate minimum stair width?**
The `determine_min_stair_width` tool takes the total number of people on the floor and a standardized module definition (like 60cm). It calculates the required width based on the ratio of population to 100, ensuring sufficient throughput for mass evacuation.

**Q: Do I need to specify the risk class when calculating extinguisher needs?**
Yes, absolutely. The `specify_extinguisher_requirement` tool requires both the total usable area and a specific risk class code (A, B, or C). This classification is mandatory because it dictates the required density and type of fire suppression equipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fire-safety-calculator](https://vinkius.com/mcp/fire-safety-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fire Safety Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fire-safety-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fire Safety Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fire-safety-calculator": {
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
