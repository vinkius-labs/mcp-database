# EdApp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edapp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Train your workforce with mobile-first microlearning courses, quizzes, and gamified lessons that employees complete on their phones.

## Description
Connect your **EdApp** (now SC Training) account to any AI agent and take full control of your corporate training and mobile learning workflows through natural conversation.

### What you can do

- **Learner Orchestration** — List and manage your learning community programmatically, including registering new users and retrieving detailed learner profiles
- **Catalog Intelligence** — Access your complete course catalog and retrieve metadata for lessons and course collections to coordinate training content
- **Success Monitoring** — Programmatically track course progress and retrieve high-fidelity analytics on completion rates and student engagement
- **Interaction Insight** — Access detailed logs of lesson attempts and user activity to identify knowledge gaps and coordinate coaching
- **Operational Visibility** — Check active webhooks and retrieve account metadata directly through your agent for instant L&D reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from the EdApp/SC Training Admin Portal (Settings > API)
3. Start managing your workforce development from Claude, Cursor, or any MCP client

No more manual status checking or digging through student lists in the portal. Your AI acts as your dedicated learning and development coordinator.

### Who is this for?

- **HR & L&D Managers** — instantly retrieve training completion reports and onboard new hires using natural language commands
- **Corporate Trainers** — monitor individual learner progress and identify lessons with high failure rates without leaving your workspace
- **Operations Leads** — automate user provisioning and training assignments through simple AI queries


## Available Tools
- **create_new_learner**: Add learner to EdApp
- **remove_learner**: Delete learner
- **get_lesson_attempts_log**: Check lesson interactions
- **list_course_lessons**: List course content
- **get_account_info**: Get admin info
- **get_course_progress_report**: Check learner progress
- **get_catalog_statistics**: Check training stats
- **get_learner_details**: Get user profile
- **list_course_collections**: List grouped content
- **list_training_courses**: List all courses
- **list_learners**: List EdApp users
- **list_active_webhooks**: Get event notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EdApp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active training courses in my EdApp account."

**🤖 AI Agent:**
> I've retrieved your course catalog. You currently have 12 active courses, including 'Cybersecurity Basics' (ID: crs_1) and 'Sales Mastery 2026'. Which one would you like to check the progress for?

---

**👤 You:**
> "Show me the progress report for course ID 'crs_1'."

**🤖 AI Agent:**
> Fetching progress for crs_1... The course has a 85% average completion rate across 50 learners. 42 users have finished all lessons, while 8 are still in progress. Shall I list the pending users?

---

**👤 You:**
> "Register 'jane.doe@example.com' as a new learner."

**🤖 AI Agent:**
> Learner created! Jane Doe has been successfully added to your EdApp workspace with ID 'usr_789'. Would you like to assign her to any specific course collections now?


## ❓ FAQ

**Q: How do I find my API Token?**
Log in to the Admin Portal, navigate to **Settings** > **API**, and generate a new Access Token for your integration.

**Q: Can I filter progress by specific courses?**
Yes! The `get_course_progress_report` tool allows you to specify a `courseId` to retrieve analytics for a particular training program.

**Q: Does it support adding new learners programmatically?**
Absolutely. Use the `create_new_learner` tool with an email address to register a new user for your training platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edapp](https://vinkius.com/mcp/edapp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EdApp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `edapp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EdApp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edapp": {
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
