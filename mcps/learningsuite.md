# LearningSuite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/learningsuite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create and deliver corporate training programs with course authoring, quizzes, and progress tracking for distributed teams.

## Description
Connect your **LearningSuite** account to any AI agent and manage training programs through natural conversation.

### What you can do

- **Course Management** — List courses, inspect syllabi, and manage content
- **Learner Tracking** — Browse learners with progress, grades, and completion data
- **Assessment Management** — Access tests, quizzes, and grading information
- **Progress Monitoring** — Track completion rates and learning paths
- **Enrollment Management** — Monitor class enrollments and roster data

### How it works

1. Subscribe to this server
2. Enter your LearningSuite API Key
3. Start managing courses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Instructors** — manage courses and track student progress
- **Training Managers** — monitor learning programs and completion rates
- **Administrators** — oversee enrollments and assessment data


## Available Tools (10)
- **get_community_post**: Get a specific community post
- **list_ai_agents**: List AI agents
- **list_courses**: List all courses
- **list_hubs**: List all hubs
- **list_members**: List all LearningSuite members
- **list_community_posts**: List all community posts
- **get_ai_agent**: Get a specific AI agent
- **get_course**: Get a specific course
- **get_hub**: Get a specific hub
- **get_member**: Get details for a specific member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LearningSuite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all courses and learner progress for the Compliance Training."

**🤖 AI Agent:**
> Courses: 5. 'Compliance Training' (85 enrolled, 72% avg completion ⭐). 'Sales Onboarding' (23, 89%). 'Product Knowledge' (45, 65%). 'Leadership Development' (12, 54%). 'Safety Certification' (34, 91%). Compliance progress: 61 completed (72%), 18 in progress, 6 not started. Average score: 84%. Deadline: May 31. ⚠️ 6 learners haven't started.

---

**👤 You:**
> "Show assessment results for the Sales Onboarding quiz."

**🤖 AI Agent:**
> Sales Onboarding Quiz: 23 submissions. Average: 87%. Pass rate: 91% (21/23 passed, 70% threshold). Top: Sarah Chen (98%), Mike Torres (95%), Lisa Park (92%). Failed: James (62%), David (58%). Questions: 25 total. Hardest: Q12 'Objection handling scenario' (52% correct). Easiest: Q1 'Product overview' (100%). Retakes allowed: 2.

---

**👤 You:**
> "Show enrollment roster and completion trends for Safety Certification."

**🤖 AI Agent:**
> Safety Certification: 34 enrolled. Completed: 31 (91% ✅). In progress: 2. Not started: 1 (Mark, enrolled Apr 20). Average completion time: 4.2 hours. Monthly trend: Jan (28 completed), Feb (30), Mar (32), Apr (31). Certification expiring: 5 within 60 days. Next recertification due: Sarah Chen, May 15.


## ❓ FAQ

**Q: Can I track learner progress and grades?**
Yes. Browse all learners with course completion percentages, assessment scores, grades, and learning path progress.

**Q: Can I access assessments and quiz results?**
Yes. Browse tests and quizzes with scores, passing rates, and individual responses for detailed analysis.

**Q: What API does LearningSuite use?**
Bearer authentication against `api.learningsuite.io/api/v1`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/learningsuite](https://vinkius.com/mcp/learningsuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LearningSuite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `learningsuite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LearningSuite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "learningsuite": {
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
