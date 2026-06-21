# Jira Cloud MCP Server

Manage projects, search issues, and track tasks via Jira Cloud API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jira-cloud)

## Overview
**Category:** industry-titans
**Tools Count:** 17

## Description
Empower your AI agents with Jira Cloud's powerful project management platform. This MCP server allows you to list and retrieve project details, search for issues using JQL, track priorities and statuses, and view dashboards directly through the Jira Cloud API. Ideal for automating software development workflows and team collaboration.


## Available Tools
- **transition_issue**: g., "To Do" → "In Progress" → "Done"). Requires a transition ID — use list_transitions to discover valid IDs for the current issue state.

Move a Jira issue to a different workflow status
- **add_comment**: The comment appears in the issue activity timeline visible to all project members.

Add a comment to a Jira issue
- **assign_issue**: Use list_users to discover account IDs. Pass an empty string to unassign.

Assign a Jira issue to a specific user
- **create_issue**: Requires the project key and a summary. Optionally set issue type (defaults to Task), description, and priority. Use list_issue_types and list_priorities to discover valid values for issuetype and priority names.

Create a new Jira issue (task, bug, story, etc.)
- **get_issue**: g., "PROJ-123"). Returns descriptions, comments, priority, status, and custom fields. Essential for providing a full context of a specific work item.

Retrieves details for a specific issue
- **get_myself**: Useful for verifying identity and permissions.

Gets current authenticated user info
- **list_projects**: Returns project keys, names, and IDs. Use this to identify project keys before searching for specific issues.

Lists all projects in Jira
- **list_sprints**: Requires the board ID which can be found in the board URL.

List sprints for a Jira agile board
- **list_statuses**: g., "To Do", "In Progress", "Done") across the Jira instance. Useful for mapping the workflow steps of projects.

Lists all issue statuses
- **list_transitions**: Use this to find transition IDs before using transition_issue.

List available workflow transitions for an issue
- **get_project**: g., "PROJ") or ID. Returns project lead, categories, and issue types. Use to understand the scope and configuration of a specific team's project.

Retrieves details for a specific project
- **list_dashboards**: Useful for identifying high-level visual reporting tools available to the user.

Lists all Jira dashboards
- **list_issue_types**: g., "Bug", "Epic", "Story") available in the Jira instance. Useful for identifying valid types when searching or creating content.

Lists all issue types
- **list_priorities**: g., "High", "Medium", "Low") configured in Jira. Useful for understanding task urgency and filtering search results.

Lists all issue priorities
- **list_users**: Use this to identify assignees, reporters, or team members by their display names or account IDs.

Lists all users in Jira
- **search_issues**: JQL allows powerful filtering (e.g., "project = MYPROJ AND status = Open"). Returns issue keys, summaries, and statuses. Use this as the main tool for finding tasks or bugs based on flexible criteria.

Searches for issues using Jira Query Language (JQL)
- **update_issue**: Provide only the fields you want to change as a JSON string.

Update fields on an existing Jira issue


## Installation & Usage

To install and use the **Jira Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jira-cloud](https://vinkius.com/mcp/jira-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
