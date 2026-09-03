# Concrete Biaxial Bending Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-biaxial-bending-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [civil-engineering](../categories/civil-engineering.md)

Design concrete columns for simultaneous axial loads and moments in two perpendicular directions.

## Description
This MCP server provides structural engineering tools to design concrete columns subjected to biaxial bending. It uses the interaction diagram method to determine if a section is safe under combined axial loads and moments (Mx and My). Users can `analyze_section_capacity` to check safety ratios, `calculate_required_reinforcement` to find the minimum steel area, `generate_reinforcement_layout` for physical bar arrangements, and `check_slenderness_effects` to account for second-order moments in slender columns.


## Available Tools (4)
- **calculate_required_reinforcement**: Finds the minimum area of steel needed to satisfy the load combination
- **check_slenderness_effects**: Evaluates if the column is "short" or "slender" and calculates the moment magnification factor
- **generate_reinforcement_layout**: Provides a physical arrangement of steel bars for the calculated required area
- **analyze_section_capacity**: Determines if the current column dimensions and material strengths can support the applied loads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Biaxial Bending Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a 300x300mm column with 30MPa concrete and 500MPa steel is safe under 1000kN axial load and 50kNm moments in both directions."

**🤖 AI Agent:**
> The capacity ratio for this column is 0.72, which means the section is safe.

---

**👤 You:**
> "How much steel area do I need for a 400x400mm column with 1500kN axial load and 80kNm moments?"

**🤖 AI Agent:**
> The required steel area is 1250 mm² with a reinforcement ratio of 0.0078.

---

**👤 You:**
> "Generate a layout for 1500mm² of steel in a 350x350mm column with 40mm cover."

**🤖 AI Agent:**
> The layout consists of 6 bars with a spacing of 120mm in both directions.


## ❓ FAQ

**Q: How do I check if my column is safe?**
Use the `analyze_section_capacity` tool. It will return a capacity ratio; if the ratio is 1.0 or less, the column is safe.

**Q: Does this tool account for slenderness?**
Yes, you can use `check_slenderness_effects` to calculate the moment magnification factor for slender columns.

**Q: Can I get a physical layout for the steel bars?**
Yes, once you have the required steel area, use `generate_reinforcement_layout` to get the bar count and spacing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-biaxial-bending-designer](https://vinkius.com/ai-agent-connect/concrete-biaxial-bending-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Biaxial Bending Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-biaxial-bending-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Biaxial Bending Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-biaxial-bending-designer": {
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
