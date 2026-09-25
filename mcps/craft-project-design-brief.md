# Craft Project Design Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/craft-project-design-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A structured planning engine that transforms raw creative intentions into actionable design specifications and execution plans.

## Description
This MCP server provides a comprehensive suite of tools to guide creators from initial idea to final handoff. Use `tool_generate_design_brief` to transform raw intentions into professional specifications, `tool_finalize_concept` to select a definitive creative path, and `tool_plan_making_sessions` to organize your work into manageable blocks. It also includes `tool_generate_quality_framework` for objective evaluation and `tool_create_handoff_plan` to prepare your finished item for its final destination.


## Available Tools (5)
- **tool_create_handoff_plan**: Prepare the item for its final destination
- **tool_finalize_concept**: Narrow down multiple creative directions into a single, actionable path
- **tool_generate_design_brief**: Transform raw user intents into a professional design specification
- **tool_generate_quality_framework**: Provide a way to objectively judge work against the original goal
- **tool_plan_making_sessions**: Total duration must not exceed totalAvailableTime.

Break down the creation process into manageable, time-bound work blocks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craft Project Design Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make a minimalist walnut jewelry box for a wedding gift. I have basic woodworking skills and want to prioritize aesthetics."

**🤖 AI Agent:**
> Design Brief: Minimalist Walnut Jewelry Box. Focus: High Aesthetic Integrity. Materials: Walnut wood, brushed brass accents. Technique: Precision joinery and fine sanding.

---

**👤 You:**
> "Help me plan my making sessions for a pottery project. I have 4 hours total and each session should be 1 hour."

**🤖 AI Agent:**
> Session 1: Clay preparation and centering. Session 2: Shaping the vessel. Session 3: Trimming and refining. Session 4: Final surface smoothing.

---

**👤 You:**
> "I've finished my project. How should I present it?"

**🤖 AI Agent:**
> Since you have confirmed the quality, here are your handoff instructions: Clean the surface thoroughly, wrap in acid-free tissue paper, and place in a custom-fitted presentation box.


## ❓ FAQ

**Q: How do I start a new project?**
You should begin by using the `tool_generate_design_brief` tool, providing your intended item and priority weights.

**Q: Can I adjust my project plan if I run out of time?**
Yes, you can use `tool_plan_making_sessions` to re-calculate your work blocks based on your updated `totalAvailableTime`.

**Q: How do I know if my project meets my quality standards?**
Use the `tool_generate_quality_framework` to receive a structured checklist of questions designed to evaluate your work against your original design brief.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/craft-project-design-brief](https://vinkius.com/en/ai-agent-connect/craft-project-design-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craft Project Design Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `craft-project-design-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craft Project Design Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craft-project-design-brief": {
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
