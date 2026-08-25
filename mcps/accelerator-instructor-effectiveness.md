# Accelerator Instructor Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-instructor-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate instructor performance scores, effectiveness trends, and get curriculum-based instructor recommendations.

## Description
This MCP server provides tools to evaluate instructor performance within accelerator programs. It calculates a comprehensive instructor score using attendance, satisfaction, and outcome correlation. You can also analyze performance trajectories with `get_effectiveness_trend` or find the best matches for upcoming sessions using `recommend_instructors` based on topic and teaching style.


## Available Tools (3)
- **get_effectiveness_trend**: Determine if an instructor's performance is improving, declining, or staying consistent
- **recommend_instructors**: Suggest the most suitable instructors for a specific upcoming curriculum or session
- **get_instructor_score**: Calculate a single, comprehensive effectiveness score for a specific instructor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Instructor Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the effectiveness score for instructor ID 'inst_99' with 90% attendance, 8.5 satisfaction, 0.7 correlation, and 50% repeat rate?"

**🤖 AI Agent:**
> The instructor 'inst_99' has a total effectiveness score of 82 and is currently categorized as 'Elite'.

---

**👤 You:**
> "Is the performance of instructor 'inst_42' improving based on these scores: 75, 80, 85?"

**🤖 AI Agent:**
> Yes, the performance for 'inst_42' is showing an 'Upward' trend with a positive momentum score.

---

**👤 You:**
> "Recommend instructors for a 'Product Management' workshop with a 'Coaching' style and a minimum score of 80."

**🤖 AI Agent:**
> I found 2 instructors matching your criteria: Sarah Jenkins and Michael Chen.


## ❓ FAQ

**Q: How is the instructor score calculated?**
The score is a weighted combination of attendance rate, student satisfaction, outcome correlation, and repeat invitation rates.

**Q: Can I find instructors for a specific topic?**
Yes, you can use `recommend_instructors` to find suitable instructors by specifying a required topic and preferred teaching style.

**Q: How do I track if an instructor is improving?**
You can use the `get_effectiveness_trend` tool by providing the instructor ID and their recent session history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-instructor-effectiveness](https://vinkius.com/ai-agent-connect/accelerator-instructor-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Instructor Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-instructor-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Instructor Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-instructor-effectiveness": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
