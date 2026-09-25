# Accessible Accessibility Review Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-accessibility-review-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms lived experience and accessibility needs into a structured, actionable Keep-Change-Stop review plan.

## Description
This MCP server acts as a reasoning engine that converts a user's current settings, routines, and support arrangements into a practical accessibility audit. By focusing on user-defined success criteria and unresolved barriers, it generates a structured Keep-Change-Stop plan. Users can use `analyze_accessibility_state` to evaluate their current situation, `generate_keep_change_stop` to create actionable items, `create_stakeholder_engagement` to prepare questions for third parties, and `construct_review_agenda` to plan future follow-ups.


## Available Tools (4)
- **analyze_accessibility_state**: Evaluate user data against success criteria and identify barriers
- **construct_review_agenda**: Build a roadmap for the next review session
- **create_stakeholder_engagement**: Generate questions for third parties to facilitate plan implementation
- **generate_keep_change_stop**: Transform analysis into a Keep-Change-Stop action plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Accessibility Review Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my current setup: I use a specialized ergonomic keyboard and a voice-to-text tool, but I struggle to navigate my desktop software quickly."

**🤖 AI Agent:**
> Your current setup provides strong input capabilities, but the software navigation is a primary barrier. We should focus on adjusting your software shortcuts or exploring new navigation tools to meet your success criteria.

---

**👤 You:**
> "Generate a review plan based on my analysis where I need to change my workstation height and stop using my current heavy mouse."

**🤖 AI Agent:**
> The plan includes: Change: Adjust workstation height to improve ergonomic alignment. Stop: Cease use of the current heavy mouse to reduce wrist strain.

---

**👤 You:**
> "What questions should I ask my landlord about installing a ramp?"

**🤖 AI Agent:**
> You should ask: 'What are the specific requirements for installing a temporary ramp at the entrance?' and 'Are there any structural guidelines I should follow to ensure compliance?'


## ❓ FAQ

**Q: Is this a medical assessment?**
No. This is a practical audit of how environments, tools, and support systems align with your specific goals and success criteria.

**Q: How does the Keep-Change-Stop framework work?**
It categorizes your current state: Keep items that meet your goals, Change items that need adjustment to reduce barriers, and Stop items that actively create obstacles.

**Q: Can I use this with Claude Desktop?**
Yes. You can connect this MCP to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-accessibility-review-plan](https://vinkius.com/en/ai-agent-connect/accessible-accessibility-review-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Accessibility Review Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-accessibility-review-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Accessibility Review Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-accessibility-review-plan": {
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
