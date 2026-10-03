# Home Accessibility Modification Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-accessibility-modification-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Prioritizes home modifications using room measurements, accessibility needs, and budget constraints.

## Description
This MCP server provides a decision-support engine for planning home accessibility improvements. It reconciles physical room constraints with specific mobility needs and budgetary limits. Users can use `analyze_spatial_compatibility` to ensure equipment fits in a room, `calculate_phased_plan` to generate a prioritized sequence of upgrades within a budget, `identify_unmet_needs` to find gaps in the plan, and `validate_dependency_chain` to ensure modification sequences are logically sound.


## Available Tools (4)
- **analyze_spatial_compatibility**: Determines if a specific modification can physically fit and function within the provided room dimensions
- **calculate_phased_plan**: Generates a prioritized sequence of modifications that fits within the total budget while respecting dependencies
- **identify_unmet_needs**: Identifies gaps between the user's stated accessibility needs and the modifications actually included in the plan
- **validate_dependency_chain**: Verifies that the requested modification list is logically sound and does not contain impossible sequences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Accessibility Modification Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a budget of $5000. Can you plan my modifications: Grab Bar ($200, priority: Critical), Door Widening ($1500, priority: High, prerequisite: Grab Bar)?"

**🤖 AI Agent:**
> Phase 1: Grab Bar ($200). Total spent: $200. Phase 2: Door Widening ($1500). Total spent: $1700.

---

**👤 You:**
> "Will a ramp with a 150cm turning radius fit in a room that is 120cm wide?"

**🤖 AI Agent:**
> No, the modification is physically impossible because the required turning radius exceeds the room's narrowest dimension.

---

**👤 You:**
> "Check if my modification list has any circular dependencies."

**🤖 AI Agent:**
> The dependency chain is valid and contains no circular loops.


## ❓ FAQ

**Q: How does the tool handle budget constraints?**
The `calculate_phased_plan` tool organizes modifications into logical stages, ensuring high-priority items are addressed first while staying within your total budget.

**Q: Can I check if a wheelchair will fit in my bathroom?**
Yes, you can use `analyze_spatial_compatibility` by providing your room dimensions and the required footprint for the wheelchair.

**Q: What happens if my budget is too low for all my needs?**
The system will identify these as unresolved constraints and use `identify_unmet_needs` to explain which requirements could not be met due to budget exhaustion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-accessibility-modification-planner](https://vinkius.com/en/ai-agent-connect/home-accessibility-modification-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Accessibility Modification Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-accessibility-modification-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Accessibility Modification Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-accessibility-modification-planner": {
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
