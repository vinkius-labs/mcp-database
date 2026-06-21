# Basecamp MCP Server

Keep your team aligned with project discussions, to-do lists, file sharing, and schedules all in one calm workspace.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/basecamp-alternative)

## Overview
**Category:** productivity
**Tools Count:** 17

## Description
Connect your **Basecamp** account to any AI agent and take full control of your project management, team collaboration, and task tracking through natural conversation.

### What you can do

- **Project Management** — Create, list, update, and inspect projects with full dock metadata (message boards, to-do sets, schedules).
- **To-Do CRUD** — Create, update, complete, and uncomplete to-do items across any to-do list, with assignees and due dates.
- **Team Visibility** — List all people in your account or within a specific project to find assignee IDs and check roles.
- **Message Boards** — Read messages posted on project boards to stay aligned with team decisions and announcements.
- **Comments** — Add comments to any recording (to-do, message, document) to provide feedback or status updates.
- **Profile Verification** — Retrieve your authenticated profile to confirm connectivity and check access permissions.

### How it works

1. Subscribe to this server
2. Enter your Basecamp OAuth access token and account ID
3. Start managing your projects from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — create tasks, assign team members, and track completion status through simple AI commands.
- **Team Leads** — monitor project boards, review messages, and add comments without switching context.
- **Remote Teams** — stay synchronized by querying project states and to-do progress directly from the workspace.


## Available Tools
- **complete_todo**: This is separate from archiving or trashing — a completed to-do remains active but is marked as done. Use uncomplete_todo to reverse this action.

Mark a to-do item as completed
- **create_comment**: ). The recording_id is the unique numeric ID of the item you want to comment on. The content must be provided as rich text (HTML). All subscribers to the recording will be notified of the new comment.

Add a comment to any Basecamp recording
- **create_project**: The project will be initialized with default tools (message board, to-do set, schedule, etc.) enabled via its dock. Returns the newly created project with its numeric ID and dock tool IDs.

Create a new project in Basecamp
- **create_todo**: Requires the todolist_id and the content (title) of the to-do. Optionally include a rich text description, assignee IDs (array of person IDs), and a due date in YYYY-MM-DD format. The to-do will be created as pending (not completed).

Create a new to-do item in a to-do list
- **get_message**: Get full details of a specific message
- **get_my_profile**: Use this to verify connectivity or identify the current operator.

Get the authenticated Basecamp user profile
- **get_person**: Use this to look up details about a team member or assignee.

Get full details of a specific person
- **get_project**: ). The dock contains the IDs you need to access tools like the to-do set or message board.

Get full details of a specific project
- **get_todo**: Get full details of a specific to-do item
- **list_messages**: Each message includes title, content preview, author, category, and creation date. You need the message_board_id which can be found via the project dock.

List all messages on a project message board
- **list_people**: Useful for finding assignee IDs before creating or updating to-dos.

List all people in the Basecamp account
- **list_project_people**: Returns names, emails, and roles. Useful for checking team composition before assigning tasks.

List all people assigned to a specific project
- **list_projects**: Optionally filter by status: "active" (default), "archived", or "trashed". Each project includes its name, description, purpose, dock (enabled tools), and bookmark status.

List all projects in Basecamp
- **list_todos**: By default returns only pending (not completed) items. Set completed to true to see completed items instead. Each to-do includes its content, assignees, due date, completion status, and comments count. You need the todolist_id which can be found via the project dock.

List all to-dos in a specific to-do list
- **uncomplete_todo**: Use this when a previously completed task needs to be reopened or reworked.

Mark a completed to-do item as pending again
- **update_project**: At least one of name or description must be provided. Returns the updated project details including the full dock listing.

Update an existing project in Basecamp
- **update_todo**: At least one field must be provided. Does not affect completion status — use the complete_todo or uncomplete_todo tools for that.

Update an existing to-do item in Basecamp


## Installation & Usage

To install and use the **Basecamp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basecamp-alternative](https://vinkius.com/mcp/basecamp-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
