# Natural Light Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/natural-light-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Calculate minimum required window dimensions for natural light and ventilation, ensuring compliance with international building standards.

## Description
**The Challenge of Passive Design**

Designing a habitable space requires more than just square footage; it demands sufficient natural light and cross-ventilation. Current building codes (like NBR 15575) mandate specific area ratios for openings, but translating these abstract minimums into physically buildable window dimensions is difficult.

**How This System Works**

The Natural Light Estimator addresses this gap by providing a structured workflow that connects code requirements to actionable architectural specifications. It uses specialized tools:

1.  `estimate_light_level`: Calculates the theoretical lux level based on input window and room areas, helping assess immediate light impact.
2.  `normalizeAreaToWindowDimensions`: This core tool takes a required minimum area (e.g., 1/6 of floor space) and calculates optimal width and height dimensions that are structurally plausible for US/EU markets.
3.  `classify_lighting`: Provides context by classifying the resulting lux level into categories like 'adequate' or 'dim', helping pinpoint specific areas needing attention.

**The Advantage**

The system synthesizes these calculations using `generateRoomSpecificationReport` to produce a single, comprehensive report. This report gives architects and builders not just theoretical minimums, but concrete, dimensioned window specifications that meet code while remaining physically feasible for construction.


## Available Tools (3)
- **estimate_light_level**: Estimate natural light level in a room based on window area, room area, and latitude
- **classify_lighting**: Classify a lux level into dark, dim, adequate, or bright category
- **recommend_improvements**: Recommend improvements for a given lighting category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Natural Light Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a specification report for a house with three rooms: Living Room (50 sqm), Kitchen (25 sqm), and Master Bedroom (30 sqm)."

**🤖 AI Agent:**
> The system will first call `generateRoomSpecificationReport`, which internally uses `calculateRoomMinimums` to find the minimum areas, then determines specific dimensions using `normalizeAreaToWindowDimensions` for all rooms and openings. The final report provides actionable measurements.

---

**👤 You:**
> "I have a 40 sqm living room and want to know the natural light level if I use a 3m x 1.5m window."

**🤖 AI Agent:**
> The system will first run `estimate_light_level` with the specified dimensions (Window Area: 4.5 sqm, Room Area: 40 sqm) and latitude to give a lux estimate. Then, you can use `classify_lighting` on that result for immediate feedback.

---

**👤 You:**
> "What improvements should I make to a room where the light level is classified as 'dim'?"

**🤖 AI Agent:**
> You can use the `recommend_improvements` tool, passing in 'dim' as the category. This will return concrete suggestions for increasing natural light or improving window placement.


## ❓ FAQ

**Q: What is the difference between minimum area and window dimensions?**
The system first calculates a 'minimum area' (e.g., 1/6 of floor space). The `normalizeAreaToWindowDimensions` tool then takes this abstract minimum and determines the most structurally sound width and height that achieves or exceeds that required area.

**Q: Can I use these tools for a whole building, not just one room?**
Yes. The `generateRoomSpecificationReport` tool accepts an array of multiple rooms and processes them sequentially. This allows you to generate a full specification report for every space in your floor plan.

**Q: What if the required minimum area is too large for standard windows?**
The `normalizeAreaToWindowDimensions` tool includes checks against physical feasibility. If a calculation results in dimensions that are structurally questionable or too large for typical openings, it will issue a warning flag within the final report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/natural-light-estimator](https://vinkius.com/mcp/natural-light-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Natural Light Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `natural-light-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Natural Light Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "natural-light-estimator": {
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
