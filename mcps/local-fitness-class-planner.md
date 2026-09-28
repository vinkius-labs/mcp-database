# Local Fitness Class Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-fitness-class-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Evaluates local fitness classes against your constraints, accessibility needs, and provider policies.

## Description
This MCP server acts as a decision-support engine for finding the perfect fitness session. It analyzes available class options against your specific constraints, such as budget, location, and schedule. By using tools like `evaluate_class_selection` and `check_availability_conflict`, it ensures that any recommended class is viable, accessible, and free of scheduling overlaps. It also generates detailed enrollment plans and logistical checklists via `generate_enrollment_plan` and `prepare_session_logistics` to ensure you are fully prepared for your first session.


## Available Tools (4)
- **check_availability_conflict**: Verify if a proposed class time overlaps with existing commitments
- **evaluate_class_selection**: Determine which class options best align with user constraints and provider rules
- **generate_enrollment_plan**: Prepare the user for the administrative side of joining a class
- **prepare_session_logistics**: Generate a checklist for the user's first session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Fitness Class Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to find a yoga class near downtown that costs less than $20 and is accessible for wheelchair users. Here are my current commitments: [Work 9am-5pm]."

**🤖 AI Agent:**
> I found a 'Gentle Flow Yoga' session at the Downtown Wellness Center for $15. It is wheelchair accessible and starts at 6:00 PM, which avoids your work commitment.

---

**👤 You:**
> "What should I prepare for my first HIIT session at the local gym?"

**🤖 AI Agent:**
> You should arrive 15 minutes early to sign waivers. Please bring water, a towel, and wear athletic clothing. The gym provides standard weights, but you may want to bring your own gloves.

---

**👤 You:**
> "Will the Tuesday 5 PM Pilates class conflict with my existing gym session on Tuesdays at 4:30 PM?"

**🤖 AI Agent:**
> Yes, there is a conflict. Your existing gym session ends at 5:30 PM, which overlaps with the start of the Pilates class.


## ❓ FAQ

**Q: How does the tool handle scheduling conflicts?**
The `check_availability_conflict` tool compares the proposed class time against your existing commitments to identify any overlaps.

**Q: Can I prepare for my first class session?**
Yes, the `prepare_session_logistics` tool generates a specific checklist including arrival instructions, equipment needs, and accessibility notes.

**Q: Does it consider my physical accessibility needs?**
Absolutely. The `evaluate_class_selection` tool specifically checks if class options satisfy your stated access needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-fitness-class-planner](https://vinkius.com/en/ai-agent-connect/local-fitness-class-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Fitness Class Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-fitness-class-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Fitness Class Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-fitness-class-planner": {
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
