# Feldenkrais Lesson Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/feldenkrais-lesson-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Design specialized Awareness Through Movement (ATM) lessons based on functional goals and physical constraints.

## Description
This MCP server provides practitioners with tools to design Feldenkrais Awareness Through Movement (ATM) lessons. Use `plan_atm_lesson` to generate complete movement sequences with precise timing and rest periods. You can use `get_variation_options` to adjust specific movements for client comfort, `validate_lesson_safety` to ensure sequences respect physical limitations, and `summarize_lesson_progress` to review the physiological impact of a plan.


## Available Tools (4)
- **get_variation_options**: Suggests ways to modify a specific movement within a sequence
- **plan_atm_lesson**: Generates a complete Feldenkrais Awareness Through Movement lesson plan
- **summarize_lesson_progress**: Provides a high-level overview of the lesson structure and impact
- **validate_lesson_safety**: Checks a proposed movement sequence against client limitations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feldenkrais Lesson Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 20-minute supine lesson focused on pelvic stability for a client with lower back stiffness."

**🤖 AI Agent:**
> I have generated a 20-minute supine lesson plan focused on pelvic stability. The sequence includes gentle pelvic tilts and hip rotations, followed by integration periods to ensure the nervous system processes the movement.

---

**👤 You:**
> "How can I make a pelvic tilt movement easier for someone with limited hip mobility?"

**🤖 AI Agent:**
> To reduce the range of motion, you can perform the pelvic tilt with a much smaller, micro-movement of the pelvis, focusing only on the sensation of weight shifting rather than visible movement.

---

**👤 You:**
> "Summarize the lesson plan with ID lesson_123."

**🤖 AI Agent:**
> Lesson lesson_123 is a 15-minute seated sequence designed to improve scapular mobility through progressive shoulder rotations and integration pauses.


## ❓ FAQ

**Q: How do I create a new lesson plan?**
Use the `plan_atm_lesson` tool by providing the functional focus, duration, and required position.

**Q: Can I modify a movement if it is too difficult for a client?**
Yes, use the `get_variation_options` tool to find alternative ways to perform a movement.

**Q: How can I ensure a lesson is safe for a client with injuries?**
You should use the `validate_lesson_safety` tool, which checks movement sequences against specific client limitations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/feldenkrais-lesson-planner](https://vinkius.com/en/ai-agent-connect/feldenkrais-lesson-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feldenkrais Lesson Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feldenkrais-lesson-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feldenkrais Lesson Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feldenkrais-lesson-planner": {
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
