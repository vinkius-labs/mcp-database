# course-progress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/course-progress)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates course completion percentages and lesson progress details.

## Description
This MCP server provides tools to track learner progress within educational courses. It allows AI agents to calculate the exact completion percentage, retrieve detailed lesson counts (total, completed, and remaining), identify upcoming progress milestones, and verify the integrity of course data for accurate calculations. Use `get_course_completion` for a quick percentage check or `get_lesson_progress_details` for a full breakdown of lesson status.


## Available Tools (4)
- **get_completion_milestones**: Retrieves upcoming progress milestones
- **get_course_completion**: Calculates the percentage of course completion
- **get_lesson_progress_details**: Gets detailed lesson progress for a course
- **verify_course_integrity**: Verifies course data integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **course-progress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the completion percentage for course ID 'math-101'?"

**🤖 AI Agent:**
> The completion percentage for course 'math-101' is 75%.

---

**👤 You:**
> "How many lessons are remaining in the 'history-basics' course?"

**🤖 AI Agent:**
> There are 3 lessons remaining in the 'history-basics' course.

---

**👤 You:**
> "Show me the progress milestones for course 'science-01' at 20% intervals."

**🤖 AI Agent:**
> The milestones for 'science-01' are 20%, 40%, and 60%.


## ❓ FAQ

**Q: How is the completion percentage calculated?**
The percentage is calculated by dividing the number of completed lessons by the total number of lessons in the course, then multiplying by one hundred.

**Q: Can I see how many lessons are left in a course?**
Yes, you can use the `get_lesson_progress_details` tool to see the total, completed, and remaining lessons.

**Q: What happens if a course has no lessons?**
If a course contains zero total lessons, the tool will return an error as progress cannot be calculated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/course-progress](https://vinkius.com/en/ai-agent-connect/course-progress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **course-progress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `course-progress` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **course-progress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "course-progress": {
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
