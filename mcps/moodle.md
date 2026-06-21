# Moodle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moodle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moodle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moodle-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Manage your Learning Management System via Moodle — track courses, users, assignments, and grades directly from your AI agent.

## Description
Connect your **Moodle** LMS account to your AI agent and streamline your educational and course management workflows through natural conversation.

### What you can do

- **Course Management** — List all courses available to your web service user and view high-level details.
- **User & Enrollment Oversight** — Search for students or teachers and list all users enrolled in a specific course.
- **Activity Tracking** — Access all quiz, assignment, and workshop activities within your courses.
- **Progress Monitoring** — Check course completion status for individual users and retrieve detailed gradebook data.
- **Group Tracking** — View all user groups defined within your courses.
- **Direct Messaging** — Send instant messages to any Moodle user ID directly from your chat.

### How it works

1. Subscribe to this server
2. Enter your Moodle Web Service Token and Site Base URL
3. Start managing your LMS from Claude, Cursor, or any MCP client

### Who is this for?

- **Teachers & Educators** — quickly check enrollment lists, assignment statuses, or send messages to students without navigating the Moodle UI.
- **LMS Administrators** — monitor courses, activities, and user profiles through natural language commands.
- **Academic Analysts** — automate the retrieval of grade and completion data for student performance reporting.


## Available Tools
- **get_course_assignments**: List assignments in courses
- **get_course_completion**: Get course completion status
- **get_course_groups**: List groups in a course
- **get_courses**: List Moodle courses
- **get_enrolled_users**: List users in a course
- **get_course_grades**: Get course grades
- **get_course_quizzes**: List quizzes in courses
- **get_users**: Search for Moodle users
- **get_course_workshops**: List workshops in courses
- **send_message**: Send an instant message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moodle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available Moodle courses."

**🤖 AI Agent:**
> I've retrieved your courses. You have access to 3 courses: 'Introduction to Computer Science', 'Advanced Mathematics', and 'World History'. Would you like to see the list of students enrolled in 'Introduction to Computer Science'?

---

**👤 You:**
> "What are the grades for students in course ID 5?"

**🤖 AI Agent:**
> Retrieving gradebook for course 5... I've found 12 students. Top performers include 'Alice Smith' (95%), 'Bob Jones' (88%), and 'Charlie Brown' (92%). Would you like the full breakdown for any specific student?

---

**👤 You:**
> "Check if user 'John Doe' (ID: 123) has finished the 'Cybersecurity' course (ID: 8)."

**🤖 AI Agent:**
> I've checked the completion status for John Doe in course 8. His progress is currently at 85%. He has completed all video lectures but still needs to submit the final project. Shall I send him a reminder message?


## Installation & Usage

To install and use the **Moodle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moodle](https://vinkius.com/mcp/moodle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
