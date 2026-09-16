# Surf School Curriculum Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-school-curriculum-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Generates structured surf lesson plans, skill progression paths, and assessment rubrics.

## Description
This MCP server provides specialized tools for surf instructors and school managers to design professional training programs. Use `generate_curriculum_framework` to build a high-level roadmap, `create_lesson_plans` for daily session details, `map_skill_progression` to visualize student growth, and `generate_assessment_rubric` to establish grading criteria based on specific learning objectives.


## Available Tools (4)
- **create_lesson_plans**: Breaks down the curriculum into granular, actionable daily instructions
- **generate_curriculum_framework**: Creates the high-level structural roadmap for a surf program
- **map_skill_progression**: Visualizes the step-by-step technical evolution a student undergoes
- **generate_assessment_rubric**: Produces the criteria used to grade or certify a student performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf School Curriculum Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 5-day beginner program for children focusing on balance and pop-ups."

**🤖 AI Agent:**
> I have generated a 5-day curriculum framework for children at Level 1 (Beginner). The program includes milestones for basic stability, paddling efficiency, and the successful execution of the pop-up maneuver.

---

**👤 You:**
> "Show me the technical progression for an intermediate surfer learning wave selection."

**🤖 AI Agent:**
> The progression path for Level 2 (Intermediate) starts with basic wave observation, moves to timing the takeoff, and concludes with mastering directional control within the wave face.

---

**👤 You:**
> "Generate a rubric for assessing advanced surfers on high-performance maneuvers."

**🤖 AI Agent:**
> The assessment rubric for Level 3 (Advanced) includes competencies for carving, speed maintenance, and technical maneuver execution with specific success thresholds for each.


## ❓ FAQ

**Q: How do I start a new surf program?**
You should start by using the `generate_curriculum_framework` tool with your target audience, duration, and desired skills.

**Q: Can I create daily schedules for my students?**
Yes, once you have a framework, use `create_lesson_plans` to generate granular daily instructions.

**Q: How are students evaluated?**
You can use `generate_assessment_rubric` to create specific grading criteria based on the skill level and objectives defined in your program.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-school-curriculum-designer](https://vinkius.com/en/ai-agent-connect/surf-school-curriculum-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf School Curriculum Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-school-curriculum-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf School Curriculum Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-school-curriculum-designer": {
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
