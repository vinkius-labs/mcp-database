# Sustainable Renovation Material Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sustainable-renovation-material-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Rank renovation materials by environmental impact, cost, and durability.

## Description
This MCP server provides tools to evaluate and rank construction materials for sustainable renovation projects. Use `get_material_catalog` to browse available options, `validate_project_parameters` to ensure your inputs are correct, and `calculate_material_rankings` to generate a prioritized list based on cost, sustainability, durability, and waste reduction. You can also use `compare_material_profiles` for deep-dive comparisons between specific materials.


## Available Tools (4)
- **calculate_material_rankings**: Generates a ranked list of materials based on a specific project's requirements
- **compare_material_profiles**: Provides a side-by-side detailed comparison of two or more specific materials
- **get_material_catalog**: Retrieves the full list of available renovation materials and their base properties
- **validate_project_parameters**: Checks if a set of user-provided project parameters is logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sustainable Renovation Material Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available flooring materials."

**🤖 AI Agent:**
> Here are the available flooring materials: Bamboo Flooring, Recycled Plastic Tiles, and Polished Concrete.

---

**👤 You:**
> "Rank these materials for a project needing 50 units: Bamboo Flooring and Recycled Plastic Tiles. I care most about sustainability."

**🤖 AI Agent:**
> Based on your priority for sustainability, Recycled Plastic Tiles ranked 1st with a score of 85, followed by Bamboo Flooring at 72.

---

**👤 You:**
> "Compare the profiles of Bamboo Flooring and Polished Concrete."

**🤖 AI Agent:**
> Bamboo Flooring has a higher recycled content and lower cost, while Polished Concrete offers significantly higher durability and a lower waste rate.


## ❓ FAQ

**Q: How are the materials ranked?**
Materials are ranked using a weighted scoring model that considers cost, sustainability (recycled content and delivery distance), durability, and waste rates.

**Q: Can I prioritize sustainability over cost?**
Yes, you can assign specific weights to different criteria using the ranking tool to shift the priority of the results.

**Q: What materials are available in the catalog?**
The catalog includes standard, eco-friendly, and premium long-life materials across various categories like flooring and insulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sustainable-renovation-material-planner](https://vinkius.com/en/ai-agent-connect/sustainable-renovation-material-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sustainable Renovation Material Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sustainable-renovation-material-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sustainable Renovation Material Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sustainable-renovation-material-planner": {
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
