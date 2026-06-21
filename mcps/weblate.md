# Weblate MCP Server

Automate localization workflows via Weblate — manage projects, components, languages, and users directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/weblate)

## Overview
**Category:** developer-tools
**Tools Count:** 32

## Description
Connect your **Weblate** instance to any AI agent to streamline your continuous localization and translation management through natural conversation.

### What you can do

- **Project & Component Management** — List all projects, fetch component details, and explore translation files directly from the Weblate API.
- **Language Insights** — Retrieve detailed statistics for specific languages to track translation progress and identify missing strings.
- **User & Group Administration** — Manage user profiles, list contributions, and handle group roles or administrative permissions.
- **Repository Operations** — Perform critical repository actions like pulling updates or pushing translations to keep your version control in sync.
- **Notification Control** — List and manage user notification subscriptions to stay updated on translation changes.

### How it works

1. Subscribe to this server
2. Enter your Weblate Instance URL and Personal API Token
3. Start managing your localization projects from Claude, Cursor, or any MCP-compatible client

No more switching between your IDE and the Weblate dashboard to check translation status or user permissions. Your AI acts as a localization manager.

### Who is this for?

- **Localization Managers** — quickly check project health, language coverage, and user contributions without manual reporting.
- **Developers** — trigger repository syncs and inspect component structures directly from the code editor.
- **DevOps Engineers** — automate user provisioning and group role assignments within the localization infrastructure.


## Available Tools
- **add_group_admins**: Add team administrators to a group
- **add_group_roles**: Associate roles with a group
- **create_group**: Create a new group
- **create_language**: Create a new language definition
- **create_project_component**: Create a new component in a project
- **create_project**: Create a new project
- **create_role**: Create a new role with specific permissions
- **create_user**: Create a new Weblate user
- **delete_user**: Delete a user (marks inactive)
- **get_group**: Get group details (roles, projects, components)
- **get_language**: Get language details (plural formulas, aliases)
- **get_project**: Get project details
- **get_role**: Get role details and permission codenames
- **get_user**: Get detailed user information
- **list_groups**: List Weblate groups
- **get_language_statistics**: Global statistics for a language
- **list_languages**: List all languages
- **list_user_notifications**: List user notification subscriptions
- **manage_user_notifications**: Manage user notification subscriptions
- **list_project_components**: List components within a project
- **get_project_file_url**: Get the URL to download all translations as a ZIP archive
- **list_project_labels**: Manage project labels
- **list_project_languages**: Paginated statistics for all languages in a project
- **perform_repository_operation**: Perform VCS operations (push, pull, commit, reset, cleanup)
- **get_project_repository**: Overall VCS status for the project
- **list_projects**: List all projects
- **list_roles**: List roles associated with the user
- **get_root**: Get Weblate API root entry point
- **update_user**: Update user details
- **get_user_contributions**: List translations with user contributions
- **get_user_statistics**: Get user translation statistics
- **list_users**: Requires management permissions or returns self.

List Weblate users


## Installation & Usage

To install and use the **Weblate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weblate](https://vinkius.com/mcp/weblate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
