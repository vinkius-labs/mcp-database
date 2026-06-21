# DingTalk MCP Server

Alibaba's B2B office platform — manage users, departments, send notifications, track attendance, and automate approval workflows.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dingtalk)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **DingTalk (钉钉)** enterprise account to any AI agent and transform your office operations through natural conversation. DingTalk is Alibaba's comprehensive B2B communication and collaboration platform used by millions of organizations for messaging, attendance tracking, approval workflows, and organizational management.

### What you can do

- **User Management** — Query employee profiles, search users by department, and retrieve contact details instantly
- **Department Exploration** — Navigate organizational hierarchy, list departments and sub-departments, understand reporting structures
- **Work Notifications** — Send text and markdown formatted messages to employees with rich formatting and clickable links
- **Attendance Tracking** — Retrieve check-in/check-out records, verify timesheet data, monitor late arrivals and early departures
- **Approval Workflows** — Create new approval instances (leave requests, reimbursements, purchases) and track their progress
- **Approval Status** — Query approval process history, identify bottlenecks, and review decision chains
- **Markdown Reports** — Send beautifully formatted markdown reports, alerts, and summaries to team members

### How it works

1. Subscribe to this server
2. Enter your DingTalk App Key and App Secret
3. Start managing your office operations from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your office operations assistant, handling user lookups, sending formatted notifications, monitoring attendance, and tracking approvals without opening the DingTalk app.

### Who is this for?

- **HR Teams** — Monitor attendance patterns, verify timesheets, and send policy announcements
- **Department Managers** — Quickly query team rosters, send formatted updates, and track approval workflows
- **Operations Leaders** — Navigate organizational structures, identify reporting lines, and broadcast markdown reports
- **Administrators** — Automate routine notifications and approval processes through conversational AI


## Available Tools
- **create_approval_process**: g., leave request, reimbursement, purchase order) by creating a new approval instance. Requires the approval template code (process_code) from your DingTalk admin, form component values matching the template structure, and the originator's user ID. Returns the process instance ID for tracking. Use this to automate approval workflows directly from AI conversations.

Create a new approval workflow instance in DingTalk
- **get_approval_instance**: Returns whether the approval is pending, approved, rejected, or cancelled, along with all reviewer actions and timestamps. Use the process instance ID obtained when creating the approval or from the approval list. Critical for tracking approval progress and understanding bottlenecks.

Get status and details of an approval process instance
- **get_attendance_records**: Returns timestamps, checkout types (上班签到/下班签退), location data, and whether the attendance was normal or abnormal (late/early leave). Essential for HR teams to monitor attendance patterns, verify timesheet data, or investigate attendance discrepancies. Date format: YYYY-MM-DD.

Get employee attendance/checkout records from DingTalk
- **get_department_info**: Use this to understand organizational hierarchy, identify department leaders, or map the reporting structure before making decisions about notification routing.

Get detailed information about a DingTalk department
- **get_user_info**: Use the user ID (userid) which can be obtained from the department user list. Essential for looking up employee details before sending targeted notifications or checking organizational structure.

Get DingTalk user profile information by user ID
- **list_all_departments**: This is the fastest way to understand the organizational structure, identify department IDs for further queries, and map team hierarchies. Use this before querying users or sub-departments to identify the correct department IDs.

List all top-level departments in the DingTalk organization
- **list_sub_departments**: Essential for exploring organizational structure, identifying team subdivisions, or mapping the complete departmental hierarchy. Start with department_id 1 to list all top-level departments in your organization.

List all sub-departments under a parent department
- **list_users_by_department**: Returns user IDs, names, avatars, and basic profile information. Useful for identifying team members before sending group notifications, checking team composition, or understanding departmental structure. Use department ID 1 for the root company directory.

List all users in a specific DingTalk department
- **send_markdown_message**: Ideal for sending structured reports, formatted alerts, or detailed notifications with clickable links. The title appears as the notification header, while the text body supports full markdown syntax including **bold**, *italic*, [hyperlinks](url), and line breaks. User IDs should be comma-separated.

Send a rich formatted markdown message to DingTalk users
- **send_work_notification**: Supports text and markdown message types. The message appears in the recipient's DingTalk work notification feed. User IDs should be comma-separated for multiple recipients. This is ideal for sending alerts, reminders, task assignments, or status updates to team members directly through DingTalk.

Send a work notification message to DingTalk users


## Installation & Usage

To install and use the **DingTalk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dingtalk](https://vinkius.com/mcp/dingtalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
