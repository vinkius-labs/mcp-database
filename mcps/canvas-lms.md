# Canvas LMS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/canvas-lms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/canvas-lms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/canvas-lms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage Canvas LMS courses, assignments, and users directly through your AI agent — streamline educational workflows and administrative tasks.

## Description
Connect your **Canvas LMS** instance to any AI agent to automate course administration and student management through natural conversation.

### What you can do

- **Course Management** — List, create, update, or delete courses. Fetch detailed metadata for specific course IDs.
- **Account Administration** — Navigate account hierarchies, list sub-accounts, and update organizational details.
- **User Operations** — Create and update user profiles, or retrieve specific user details and activity streams.
- **Assignments & Tasks** — List all assignments within a course and track your personal 'To Do' items and activity stream.
- **Workflow Automation** — Use your AI as a teaching assistant or admin to handle repetitive setup tasks in the LMS.

### How it works

1. Subscribe to this server
2. Enter your Canvas Domain (e.g., school.instructure.com) and Personal Access Token
3. Start managing your virtual classroom from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Educators & Tutors** — quickly check assignment lists or update course details without navigating complex menus
- **LMS Administrators** — automate user creation and account management across sub-accounts
- **Students & Developers** — track personal todos and activity streams directly from the terminal or code editor


## Available Tools
- **create_admin**: Make a user an admin in an account
- **create_assignment**: Create a new assignment in a course
- **create_conversation**: Create a new conversation
- **create_course**: Create a new Canvas course
- **create_discussion_topic**: Create a new discussion topic in a course
- **create_quiz**: Create a new quiz in a course
- **create_role**: Create a new role in an account
- **create_sis_import**: Import SIS data
- **create_user**: Create a new Canvas user
- **delete_course**: Delete or conclude a Canvas course
- **execute_graphql**: Execute a GraphQL query against Canvas
- **get_account**: Get details for a specific Canvas account
- **get_activity_stream**: Get current user activity stream
- **get_assignment**: Get details for a specific assignment
- **get_conversation**: Get details for a specific conversation
- **get_course**: Get details for a specific Canvas course
- **get_file**: Get details for a specific file
- **get_folder**: Get details for a specific folder
- **get_page**: Get details for a specific page
- **get_quiz**: Get details for a specific quiz
- **get_sis_import_status**: Get status of a SIS import
- **get_sub_accounts**: Get sub-accounts for a specific account
- **get_todo**: Get current user todo items
- **get_user**: Show user details
- **grade_submission**: Grade a submission
- **list_accounts**: List Canvas accounts
- **list_admins**: List admins in an account
- **list_announcements**: List announcements
- **list_assignments**: List assignments for a course
- **list_conversations**: List conversations (Inbox)
- **list_courses**: List your Canvas courses
- **list_discussion_topics**: List discussion topics in a course
- **list_files**: List files in a course
- **list_folders**: List sub-folders within a folder
- **list_module_items**: List items in a specific module
- **list_modules**: List modules in a course
- **list_pages**: List pages in a course
- **list_quizzes**: List quizzes in a course
- **list_roles**: List roles in an account
- **list_submissions**: List submissions for an assignment
- **submit_assignment**: Submit an assignment
- **update_account**: Update an existing Canvas account
- **update_assignment**: Edit an existing assignment
- **update_course**: Update an existing Canvas course
- **update_user**: Update an existing Canvas user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canvas LMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Canvas courses."

**🤖 AI Agent:**
> I've retrieved your courses. You are currently enrolled in: 'Introduction to Biology' (ID: 101), 'Advanced Mathematics' (ID: 202), and 'History 101' (ID: 303).

---

**👤 You:**
> "Show me my current todo items from Canvas."

**🤖 AI Agent:**
> You have 3 items on your todo list: 'Submit Lab Report' (due tomorrow), 'Quiz: Calculus' (due Friday), and 'Peer Review: Essay' (due Sunday).

---

**👤 You:**
> "List the assignments for course ID 202."

**🤖 AI Agent:**
> For 'Advanced Mathematics' (ID: 202), I found the following assignments: 'Problem Set 1', 'Midterm Exam', and 'Final Project Proposal'.


## Installation & Usage

To install and use the **Canvas LMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canvas-lms](https://vinkius.com/mcp/canvas-lms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
