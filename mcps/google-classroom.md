# Google Classroom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-classroom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-classroom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-classroom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage classes, assignments, students, and submissions — automate your Google Classroom workflows via AI.

## Description
Connect your **Google Classroom** to any AI agent and streamline your teaching workflows through natural conversation. Manage courses, create assignments, track student submissions, and grade work — all via AI commands.

### What you can do
- **Course Management** — List, create, and update courses with full details
- **Roster Tracking** — List enrolled students and assigned teachers for any course
- **Assignments** — Create coursework, set due dates, and track all assignments
- **Submission Monitoring** — Check who turned in work, who's late, and who hasn't submitted
- **Grading** — Review individual submissions, return graded work to students
- **Announcements** — Post important updates to the course stream

### How it works
1. Subscribe to this server
2. Enter your Google Classroom OAuth Access Token
3. Start managing classes from Claude, Cursor, or any MCP client

### Who is this for?
- **Teachers** — Quickly check submissions, create assignments, and post announcements
- **Students** — Track your submissions and check grades
- **Administrators** — Monitor course rosters and assignment completion across classes


## Available Tools
- **create_announcement**: Announcements appear in the course stream and can be used for important updates, reminders, or general communication.

Post a new announcement to a Google Classroom course
- **create_course**: Returns the new course ID for future reference. Only users with appropriate permissions can create courses.

Create a new Google Classroom course
- **create_course_work**: The assignment will be visible to all students in the course. Supports assignments, quizzes, and materials types.

Create a new assignment or coursework in Google Classroom
- **get_course**: Use the course ID obtained from list_courses.

Get details of a specific Google Classroom course
- **get_submission**: Get a specific student's submission details
- **list_announcements**: Use this to check recent course announcements and important updates.

List all announcements in a Google Classroom course
- **list_course_work**: Returns assignment title, due date, state (DRAFT/PUBLISHED), max points, and creation time. Use this to track all assignments and their deadlines.

List all assignments and coursework for a Google Classroom course
- **list_courses**: Essential first step to identify which course to work with before querying students, assignments, or submissions.

List all Google Classroom courses
- **list_students**: Use this to check enrollment, identify students for grading, or verify class roster.

List all students enrolled in a Google Classroom course
- **list_submissions**: Returns student ID, submission state (NEW/CREATED/TURNED_IN/RETURNED), grade, and late status.

List student submissions for a specific assignment
- **list_teachers**: List all teachers of a Google Classroom course
- **return_submission**: This is typically done after the teacher has reviewed and graded the work. The student will be notified that their work has been returned.

Return a graded assignment to the student
- **turn_in_submission**: The student must have created the submission first. This is equivalent to clicking "Turn In" in the Classroom UI.

Turn in a student's assignment submission
- **update_course**: Requires the course ID and at least one field to update.

Update an existing Google Classroom course


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Classroom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my courses and show students in Math 101."

**🤖 AI Agent:**
> 📚 You have 3 courses: Math 101 (ID: 12345), Physics 201 (ID: 12346), Chemistry 301 (ID: 12347). Students in Math 101: Alice, Bob, Charlie, Diana (4 enrolled).

---

**👤 You:**
> "Create an assignment called 'Chapter 5 Problems' due 2024-05-15 for course 12345, max 100 points."

**🤖 AI Agent:**
> ✅ Assignment created! 'Chapter 5 Problems' (CourseWork ID: cw_789) for Math 101, due May 15, 2024, max 100 points. All students can now see the assignment.

---

**👤 You:**
> "Show me who turned in the Chapter 5 assignment."

**🤖 AI Agent:**
> 📊 Submissions for 'Chapter 5 Problems': ✅ Turned In: Alice, Bob (2) | ⏳ Late: Charlie (1) | ❌ Not Submitted: Diana (1).


## Installation & Usage

To install and use the **Google Classroom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-classroom](https://vinkius.com/mcp/google-classroom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
