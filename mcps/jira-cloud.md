# Jira Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jira-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage projects, search issues, and track tasks via Jira Cloud API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jira Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Jira."

**🤖 AI Agent:**
> I'll fetch the list of all projects you have access to in Jira.

---

**👤 You:**
> "Search for all issues assigned to 'user@example.com'."

**🤖 AI Agent:**
> I'll use JQL to find all issues assigned to that specific user.

---

**👤 You:**
> "Get details for issue 'PROJ-123'."

**🤖 AI Agent:**
> I'll retrieve the full details, including status and priorities, for that Jira issue.


## ❓ FAQ

**Q: How do I get Jira API credentials?**
You need your Jira instance domain (e.g., acme.atlassian.net), your account email, and an API Token. You can generate an API Token in your Atlassian Account Settings under Security > API Token.

**Q: What is JQL?**
JQL (Jira Query Language) is a powerful tool that allows you to search for issues in Jira using a structured query syntax.

**Q: Can I see private projects?**
Your AI agent will only be able to see projects and issues that your Atlassian account has permission to access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jira-cloud](https://vinkius.com/mcp/jira-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jira Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jira-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jira Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jira-cloud": {
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
