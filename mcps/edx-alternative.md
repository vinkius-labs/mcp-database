# edX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edx-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage Open edX courses, enrollments, and user profiles — list learning paths, track student grades, and handle registrations via AI.

## Description
Connect your **Open edX** platform to any AI agent to streamline course administration and student tracking through natural conversation.

### What you can do

- **Course Management** — List all available courses and fetch detailed metadata for specific learning paths using unique course IDs.
- **Enrollment Handling** — View current user enrollments and enroll students in new courses instantly without manual dashboard navigation.
- **Student Progress** — Retrieve grades for individual users or entire course cohorts to monitor performance and completion rates.
- **Profile Control** — Inspect and update user profiles, email addresses, and preferences directly via the API.
- **Course Structure** — Access course blocks and structural data to understand the curriculum layout and content hierarchy.

### How it works

1. Subscribe to this server
2. Enter your Open edX Base URL and Access Token
3. Start managing your LMS environment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **LMS Administrators** — quickly check enrollment numbers and course statuses without logging into the management console.
- **Instructors & Tutors** — retrieve student grades and profile information directly while providing feedback or support.
- **Developers** — inspect course block structures and user preferences while building integrations or custom themes.


## Available Tools (10)
- **get_course_grades**: Get Open edX course grades
- **get_user_grades**: Get Open edX user grades for a course
- **get_user_preferences**: Get Open edX user preferences
- **get_user_profile**: Get Open edX user profile
- **list_courses**: List Open edX courses
- **list_enrollments**: List Open edX enrollments
- **update_user_profile**: Update Open edX user profile
- **enroll_in_course**: Enroll in an Open edX course
- **get_course_blocks**: Get Open edX course blocks
- **get_course_details**: Get Open edX course details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **edX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available courses on our edX platform."

**🤖 AI Agent:**
> I've retrieved the course list. You have 3 active courses: 'Introduction to AI' (ID: course-v1:Org+AI101+2024), 'Advanced Python' (ID: course-v1:Org+PY201+2024), and 'Data Science Basics'.

---

**👤 You:**
> "Enroll me in the course course-v1:Org+AI101+2024."

**🤖 AI Agent:**
> Processing enrollment... Success! You are now enrolled in 'Introduction to AI'. You can start accessing the course materials immediately.

---

**👤 You:**
> "Show me the grades for user 'jdoe' in the Python course."

**🤖 AI Agent:**
> Fetching grades for 'jdoe'... In 'Advanced Python', the user has a current grade of 85%. All assignments are completed except for the final project which is pending.


## ❓ FAQ

**Q: Can I check a specific student's grades for a course?**
Yes. Use the `get_user_grades` tool by providing the `course_id` and the student's `username`. The agent will return the grading breakdown for that specific user.

**Q: Is it possible to enroll a user in a course via the AI?**
Absolutely. The `enroll_in_course` tool allows you to register the authenticated user into any course by specifying its unique `course_id`.

**Q: Can I update user profile information like names or emails?**
Yes, the `update_user_profile` tool enables you to modify the name or email associated with a specific username in your Open edX instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edx-alternative](https://vinkius.com/mcp/edx-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **edX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `edx-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **edX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edx-alternative": {
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
