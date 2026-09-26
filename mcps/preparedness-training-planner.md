# Preparedness Training Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/preparedness-training-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A personalized scheduler for household emergency preparedness training and practice drills.

## Description
This MCP server helps households build resilience by organizing emergency preparedness training. It manages prerequisite logic for courses, tracks certification expiration, and schedules hands-on practice drills. Use `get_learning_schedule` to create a timeline, `get_enrollment_tasks` to manage training costs, `get_practice_calendar` to schedule drills, and `get_evidence_plan` to organize your certification and drill logs.


## Available Tools (4)
- **get_practice_calendar**: Suggests dates for hands-on drills to ensure theoretical knowledge is converted into physical skill
- **get_enrollment_tasks**: Extracts a specific "to-do" list of administrative actions required to secure training
- **get_evidence_plan**: Organizes a digital or physical filing structure to store certificates and drill logs
- **get_learning_schedule**: Generates a chronological timeline of when each household member should undertake specific courses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Preparedness Training Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a learning schedule for Alice and Bob with these courses: Basic First Aid ($50), Wilderness First Aid ($150). Alice is available 2 hours a week."

**🤖 AI Agent:**
> Alice: Basic First Aid (Starts: 2024-05-01, Ends: 2024-05-07); Bob: Basic First Aid (Starts: 2024-05-01, Ends: 2024-05-07); Alice: Wilderness First Aid (Starts: 2024-05-14, Ends: 2024-05-21).

---

**👤 You:**
> "What are the enrollment tasks for Basic First Aid if my budget is $100?"

**🤖 AI Agent:**
> Task: Pay registration fee for Basic First Aid. Estimated Cost: $50.

---

**👤 You:**
> "Suggest practice dates for our completed Basic First Aid course. We are available on weekends in June."

**🤖 AI Agent:**
> Drill Type: First Aid Drill; Suggested Date: 2024-06-01; Target Skill: Basic Wound Care.


## ❓ FAQ

**Q: How does the tool handle course prerequisites?**
The `get_learning_schedule` tool automatically ensures that foundational courses are completed before any dependent advanced courses are scheduled.

**Q: Can I schedule hands-on drills?**
Yes, you can use `get_practice_calendar` to suggest specific dates for drills based on your household's availability and completed training.

**Q: How do I organize my training certificates?**
The `get_evidence_plan` tool generates a structured folder hierarchy to help you store all your certificates and drill logs systematically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/preparedness-training-planner](https://vinkius.com/en/ai-agent-connect/preparedness-training-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Preparedness Training Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `preparedness-training-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Preparedness Training Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "preparedness-training-planner": {
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
