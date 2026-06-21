# Blackboard Learn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blackboard-learn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage courses, announcements, attendance, and grades directly from your AI agent via Blackboard Learn.

## Description
Connect your **Blackboard Learn** environment to any AI agent to streamline educational management and course administration through natural conversation.

### What you can do

- **Course Management** — List all active courses, fetch specific course details, and manage user enrollments or memberships.
- **Announcements** — View system-wide announcements or create and update specific course announcements to keep students informed.
- **Attendance Tracking** — List scheduled meetings, create new attendance sessions, and mark or retrieve attendance records for users.
- **Gradebook Access** — Monitor academic performance by listing gradebook columns, fetching specific grades, and tracking recent grade changes.
- **Calendar & Scheduling** — List and create calendar items to manage deadlines and events across the academic term.
- **User Administration** — List system users, create new user profiles, and view course loads for specific individuals.

### How it works

1. Subscribe to this server
2. Enter your Blackboard Learn Base URL and Personal Access Token
3. Start managing your LMS environment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Instructors & Teachers** — quickly post announcements, check who attended class, and review recent grade updates without navigating complex menus.
- **Academic Administrators** — manage enrollments and monitor system-wide announcements across multiple departments.
- **Students & Researchers** — query course details and calendar deadlines directly from their workspace.


## Available Tools
- **create_calendar_item**: Create a calendar item
- **create_course_announcement**: Create a course announcement
- **create_meeting**: Create a new attendance meeting
- **create_user**: Create a new user
- **delete_calendar_item**: Delete a calendar item
- **enroll_user**: Enroll a user in a course
- **get_column_grades**: Get grades for a column
- **get_course**: Get course details
- **get_meeting_attendance**: Get attendance records for a meeting
- **get_recent_grade_changes**: Check for recent grade changes
- **list_system_announcements**: List system announcements
- **list_calendar_items**: List calendar items
- **list_course_memberships**: List course memberships
- **list_courses**: List courses
- **list_gradebook_columns**: List gradebook columns
- **list_meetings**: List all attendance meetings for a course
- **list_user_courses**: List courses for a specific user
- **list_users**: List users
- **mark_attendance**: Mark attendance for a user
- **update_course_announcement**: Update a course announcement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blackboard Learn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active courses in Blackboard."

**🤖 AI Agent:**
> I've retrieved your courses. You are currently enrolled in: 'Introduction to Computer Science' (ID: CS101) and 'Advanced Mathematics' (ID: MATH302). Would you like to see the details for one of them?

---

**👤 You:**
> "Create a course announcement for CS101 titled 'Final Exam Update' saying 'The exam is moved to Friday'."

**🤖 AI Agent:**
> Announcement created successfully in course CS101. Students will now see the update regarding the final exam schedule.

---

**👤 You:**
> "Show me the attendance records for meeting ID 98765 in course MATH302."

**🤖 AI Agent:**
> Fetching attendance for meeting 98765... I found 25 records. 22 students are marked as 'Present', 2 as 'Absent', and 1 as 'Late'. Would you like the specific names of the absent students?


## ❓ FAQ

**Q: How can I check the attendance records for a specific class meeting?**
You can use the `get_meeting_attendance` tool by providing the Course ID and Meeting ID. The agent will retrieve the full list of users and their current attendance status (e.g., Present, Absent).

**Q: Is it possible to see recent changes in student grades?**
Yes, use the `get_recent_grade_changes` tool. It allows you to monitor updates in the gradebook, helping you stay informed about recent evaluations and adjustments.

**Q: Can I post a new announcement to my students through the AI?**
Absolutely. Use the `create_course_announcement` tool. Just provide the Course ID, a title, and the body of your message, and the agent will publish it to the course immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blackboard-learn](https://vinkius.com/mcp/blackboard-learn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blackboard Learn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blackboard-learn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blackboard Learn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blackboard-learn": {
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
