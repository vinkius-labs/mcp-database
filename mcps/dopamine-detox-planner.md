# Dopamine Detox Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dopamine-detox-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design personalized neurochemical reset protocols to improve focus and mental clarity.

## Description
The Dopamine Detox Planner is a strategic engine designed to help you recalibrate your brain's reward system. By identifying high-stimulation habits and replacing them with healthy alternatives, you can regain control over your focus and motivation. Use `plan_restriction_list` to identify which habits to pause, `generate_replacement_schedule` to build a productive daily routine, and `get_reintroduction_roadmap` to safely reintegrate activities after your reset. This tool provides a structured path to mental clarity through regulated stimulation restriction.


## Available Tools (4)
- **plan_restriction_list**: 
- **generate_replacement_schedule**: 
- **get_detox_summary**: 
- **get_reintroduction_roadmap**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dopamine Detox Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What habits should I restrict for a high-intensity detox?"

**🤖 AI Agent:**
> Based on a high-intensity threshold, you should restrict social media scrolling, video gaming, and consumption of sugary snacks.

---

**👤 You:**
> "Help me plan my day from 08:00 to 20:00."

**🤖 AI Agent:**
> Your schedule includes morning meditation at 08:00, reading from 10:00 to 11:00, a walk at 14:00, and journaling at 19:00.

---

**👤 You:**
> "Give me a summary of my current detox plan."

**🤖 AI Agent:**
> Your protocol focuses on improving focus by restricting high-stimulation digital habits for 7 days, replacing them with physical and cognitive activities.


## ❓ FAQ

**Q: How do I know which habits to stop?**
You can use the `plan_restriction_list` tool to identify specific habits that meet your chosen stimulation intensity threshold.

**Q: Can I create a daily schedule for my detox?**
Yes, the `generate_replacement_schedule` tool creates a structured daily timeline of low-stimulation activities based on your available time windows.

**Q: What happens after my detox period ends?**
You should use `get_reintroduction_roadmap` to follow a controlled, step-by-step plan for reintegrating activities without triggering a relapse.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dopamine-detox-planner](https://vinkius.com/en/ai-agent-connect/dopamine-detox-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dopamine Detox Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dopamine-detox-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dopamine Detox Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dopamine-detox-planner": {
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
