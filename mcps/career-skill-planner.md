# Career Skill Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/career-skill-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Builds personalized learning schedules based on skills, budget, and availability.

## Description
This MCP server helps users design structured learning paths. It analyzes skill dependencies using `get_skill_dependencies`, checks if a learning plan is realistic with `calculate_feasibility`, and generates a detailed chronological roadmap via `generate_learning_schedule`. You can also use `get_skill_details` to find specific costs and time requirements for any skill in the catalog.


## Available Tools (4)
- **calculate_feasibility**: To check if a set of desired skills can realistically be learned within the user's budget and time constraints
- **generate_learning_schedule**: To create a chronological roadmap of when to study each skill
- **get_skill_dependencies**: To understand which skills must be learned before others can be started
- **get_skill_details**: To retrieve the cost and duration requirements for a specific skill


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Career Skill Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I learn Python and Data Science with a $200 budget and 5 hours available per week?"

**🤖 AI Agent:**
> Yes, that plan is feasible. Your total cost for these skills is $150, and you have enough weekly hours to complete them before the deadlines.

---

**👤 You:**
> "What are the requirements for the 'Advanced Machine Learning' skill?"

**🤖 AI Agent:**
> Advanced Machine Learning requires 40 course hours and costs $120. The target completion deadline is December 15th, 2024.

---

**👤 You:**
> "Create a study plan for 'Web Development' with 10 hours a week and a $50 budget."

**🤖 AI Agent:**
> Your learning schedule is ready. You will spend 10 hours in Week 1 on HTML/CSS and 10 hours in Week 2 on JavaScript, staying within your $50 budget.


## ❓ FAQ

**Q: How does the tool handle skill prerequisites?**
The tool uses `get_skill_dependencies` to ensure that any prerequisite skill is scheduled and completed before its dependent skill begins.

**Q: Can I plan a schedule if I have a limited budget?**
Yes. You can use `calculate_feasibility` to verify if your desired skills fit within your budget and `generate_learning_schedule` to create the plan.

**Q: What happens if my weekly availability is too low?**
If the available hours are insufficient to meet skill deadlines, `calculate_feasibility` will report a constraint violation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/career-skill-planner](https://vinkius.com/en/ai-agent-connect/career-skill-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Career Skill Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `career-skill-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Career Skill Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "career-skill-planner": {
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
