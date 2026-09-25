# Community Fundraiser Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-fundraiser-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform raw fundraising inputs into actionable, compliant execution roadmaps.

## Description
This MCP server provides a strategic planning engine for community fundraising. It transforms raw inputs--such as causes, targets, volunteers, and donor lists--into comprehensive execution roadmaps. Use `plan_fundraiser_execution` to generate timelines, role rosters, and communication plans. You can also use `audit_budget_alignment` to ensure costs stay within limits, `validate_donor_engagement` to respect privacy permissions, and `generate_milestone_triggers` to automate progress-based actions.


## Available Tools (4)
- **audit_budget_alignment**: Verifies that the proposed financial plan is within the limits and meets the target requirements
- **generate_milestone_triggers**: Determines the specific actions that must occur when certain financial or temporal thresholds are met
- **plan_fundraiser_execution**: Generates the complete strategic roadmap for the community event
- **validate_donor_engagement**: Checks if a proposed communication or outreach action respects the privacy and permission settings of specific donors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Fundraiser Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a fundraiser for a local animal shelter with a $5,000 goal and a $500 budget cap."

**🤖 AI Agent:**
> The fundraising plan for the animal shelter has been generated. The total projected costs are $450, which is within your $500 budget cap. The timeline spans 14 days, and the volunteer roster has been assigned to logistics and outreach.

---

**👤 You:**
> "Check if I can give a public shoutout to donor Jane Doe."

**🤖 AI Agent:**
> Jane Doe is listed with privacy permissions, so she cannot be included in public shoutouts.

---

**👤 You:**
> "We have raised $2,500 of our $5,000 goal. What should we do next?"

**🤖 AI Agent:**
> You have reached the 50% milestone. The triggered action is to send a progress update email to all participating donors.


## ❓ FAQ

**Q: How does the tool handle budget constraints?**
The `audit_budget_alignment` tool verifies that all proposed costs are within your specified budget cap and calculates the gap relative to your target amount.

**Q: Can I ensure donor privacy during outreach?**
Yes. By using `validate_donor_engagement`, the system checks donor permission settings to ensure actions like public shoutouts respect privacy constraints.

**Q: What kind of roadmap is generated?**
The `plan_fundraiser_execution` tool produces a full roadmap including a chronological timeline, a volunteer role roster, a communication plan, and a transparency checklist.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-fundraiser-planner](https://vinkius.com/en/ai-agent-connect/community-fundraiser-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Fundraiser Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-fundraiser-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Fundraiser Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-fundraiser-planner": {
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
