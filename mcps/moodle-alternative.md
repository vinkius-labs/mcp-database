# Moodle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moodle-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Power your e-learning environment with the world most flexible open-source LMS for course creation and student management.

## Description
Connect your **Moodle** instance to any AI agent and manage your learning platform through natural conversation.

### What you can do

- **Courses** — List, create, and browse course content sections
- **Users** — Search, create, and manage learner profiles
- **Enrolment** — Enrol users into courses and view enrolled learners
- **Grades** — Retrieve grade items and student results per course
- **Assignments** — List assignments for specific courses
- **Categories** — Browse course organization categories
- **Files** — Access files attached to course modules
- **Site Info** — Retrieve Moodle instance metadata

### How it works

1. Subscribe to this server
2. Enter your Moodle Site URL and API Token
3. Start managing courses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Educators** — automate course creation and student enrolment
- **Administrators** — bulk-manage users and grade retrieval
- **EdTech** — integrate LMS data into AI-powered workflows


## Available Tools (12)
- **get_site_info**: Get Moodle site information
- **get_user_grades**: Get grades for a user in a course
- **list_assignments**: List assignments for courses
- **list_categories**: List course categories
- **list_courses**: List all available courses
- **list_files**: List files in a specific area
- **list_users**: g., username, email) and value.

Search for users in Moodle
- **create_courses**: Requires fullname, shortname, and categoryid.

Create new courses
- **create_users**: Requires username, password, firstname, lastname, and email.

Create new users in Moodle
- **enrol_users**: Enrol users into a course
- **get_course_contents**: Get contents of a specific course
- **get_enrolled_users**: Get users enrolled in a course


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moodle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all courses and show enrolment counts."

**🤖 AI Agent:**
> Courses: 5. 1) 'Introduction to Python' (ID: 2, 45 enrolled). 2) 'Data Science Fundamentals' (ID: 3, 32 enrolled). 3) 'Web Development' (ID: 4, 28 enrolled). 4) 'Machine Learning' (ID: 5, 18 enrolled). 5) 'Database Design' (ID: 6, 52 enrolled). Total students: 175.

---

**👤 You:**
> "Get grades for student ID 42 in the Python course."

**🤖 AI Agent:**
> Grades for Student #42 in 'Introduction to Python' (Course ID: 2): 1) Quiz 1: 85/100. 2) Assignment 1: 92/100. 3) Midterm Exam: 78/100. 4) Final Project: 95/100. Course Total: 87.5%. Status: Passing.

---

**👤 You:**
> "Create a new course 'AI Ethics' in category 1 and enrol 3 students."

**🤖 AI Agent:**
> Course created! ✅ 'AI Ethics' (ID: 7, Category: General). Shortname: ai_ethics_2024. Now enrolling... ✅ 3 students enrolled with role 'Student' (Role ID: 5). All set!


## ❓ FAQ

**Q: Can I create courses and enrol students?**
Yes. Create courses with full metadata, then enrol users with specific role IDs (student, teacher, manager).

**Q: How does Moodle authentication work?**
Moodle requires your **Site URL** and an **API Token** (wstoken). The token is passed as a query parameter to the Web Service REST endpoint.

**Q: Can I retrieve student grades?**
Yes. Retrieve grade items and results for any user within a specific course using their course and user IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moodle-alternative](https://vinkius.com/mcp/moodle-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moodle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moodle-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moodle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moodle-alternative": {
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
