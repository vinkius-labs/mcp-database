# D2L Brightspace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/d2l-brightspace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your D2L Brightspace LMS — administer courses, track student grades, and manage enrollments directly through your AI agent.

## Description
Connect your **D2L Brightspace** environment to any AI agent to streamline learning management and administrative workflows.

### What you can do

- **Course Management** — Retrieve course details, create new offerings, and copy course content between org units using `get_course` and `copy_course`.
- **User Administration** — List system users, create new accounts, and manage roles and permissions with `list_users` and `create_user`.
- **Grade Tracking** — Access grade lists and update individual student grades for specific assignments using `get_user_grade` and `update_user_grade`.
- **Content & Communication** — Explore course modules, manage discussion forums, and create new topics or posts via `list_root_modules` and `create_post`.
- **Assessments** — Monitor quizzes, surveys, and assignment submissions, and provide direct feedback using `list_submissions` and `provide_feedback`.

### How it works

1. Subscribe to this server
2. Provide your Brightspace Host URL and Access Token
3. Start managing your educational ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Instructors** — Quickly check student progress, provide feedback on assignments, and manage course content without navigating complex menus.
- **LMS Administrators** — Automate user creation, enrollment management, and organizational unit structuring.
- **Academic Researchers** — Extract course data and assessment metrics for analysis through natural language queries.


## Available Tools (33)
- **copy_course**: Initiate a course copy job
- **create_course**: Create a course offering
- **create_enrollment**: Enroll a user in an org unit
- **create_lti_deployment**: Create an LTI Advantage tool deployment
- **create_org_unit**: Create custom org units
- **create_post**: Create a post in a discussion topic
- **create_topic**: Create a discussion topic in a forum
- **create_user**: Create a new user
- **delete_enrollment**: Unenroll a user from an org unit
- **get_course_template**: Retrieve course template info
- **get_course**: Retrieve course details
- **get_org_unit**: Retrieve org unit properties
- **get_user_grade**: Retrieve user grades for a specific grade object
- **list_assignment_folders**: List assignment folders (dropboxes)
- **list_forums**: List discussion forums in a course
- **list_grades**: List grade objects for a course
- **list_legacy_lti_links**: List legacy LTI 1.1 links
- **list_lti_registrations**: List LTI Advantage tool registrations
- **list_my_eportfolio_objects**: List current user ePortfolio objects
- **list_my_enrollments**: List current user enrollments
- **list_org_unit_children**: List child units of an org unit
- **list_quiz_attempts**: List attempts for a specific quiz
- **list_quizzes**: List quizzes in a course
- **list_roles**: Retrieve system roles
- **list_root_modules**: List root modules of course materials
- **list_submissions**: List submissions for an assignment folder
- **list_surveys**: List surveys in a course
- **list_users**: Search or page through users
- **provide_feedback**: Provide feedback for an assignment submission
- **update_user_grade**: Update a user grade
- **update_user**: Update user data
- **upload_eportfolio_artifact**: Upload a file artifact to ePortfolio
- **get_whoami**: Retrieve current user context


## 💬 Prompt Examples

Here are some examples of how you can interact with the **D2L Brightspace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Brightspace instance."

**🤖 AI Agent:**
> I've retrieved the user list. There are currently 150 users registered. Would you like to filter them by role or search for a specific name?

---

**👤 You:**
> "Show me the details for course org unit 8821."

**🤖 AI Agent:**
> Course Unit 8821 is 'Introduction to Computer Science'. It is currently active with 45 students enrolled. Would you like to see the root modules or the grade list for this course?

---

**👤 You:**
> "Get the grade for user 554 in course 8821."

**🤖 AI Agent:**
> User 554 (John Doe) has a current grade of 88% in course 8821. This includes 3 completed assignments and 1 pending quiz.


## ❓ FAQ

**Q: Can I check a specific student's grade for a course unit?**
Yes. By using the `get_user_grade` tool with the appropriate Org Unit ID and User ID, the agent can retrieve the current grade details for that student.

**Q: Is it possible to list all modules within a course structure?**
Absolutely. Use the `list_root_modules` tool to fetch the top-level content structure for any specific course org unit.

**Q: Can I manage discussion forums through this agent?**
Yes, you can use `list_forums` to see available forums and `create_topic` or `create_post` to interact with the discussion boards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/d2l-brightspace](https://vinkius.com/mcp/d2l-brightspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **D2L Brightspace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `d2l-brightspace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **D2L Brightspace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "d2l-brightspace": {
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
