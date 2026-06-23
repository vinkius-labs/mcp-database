# GitLab MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitlab)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage projects, track issues, and oversee CI/CD pipelines via AI agents with GitLab.

## Description
Connect your **GitLab** instance to any AI agent to automate your DevSecOps lifecycle and project management through the Model Context Protocol (MCP). GitLab is the most comprehensive AI-powered platform for software innovation. This MCP server enables you to retrieve project metadata, manage issues, track merge requests, and monitor CI/CD pipelines directly through natural conversation.

### Key Features

- **Project Oversight** — List all accessible projects, fetch detailed configuration metadata, and track forks across your instance.
- **Issue & MR Management** — List issues and merge requests, track their lifecycle status, and programmatically open new issues from your chat interface.
- **CI/CD Visibility** — Retrieve a list of pipelines for any project to monitor build and deployment health in real-time.
- **Repository Discovery** — Access the contents of files within any repository to understand codebase structures and documentation.
- **Global Search** — Execute powerful searches across projects, issues, and users to isolate specific development artifacts.
- **Identity Oversight** — Access detailed profile information for the authenticated user to verify permissions and account context.
- **Real-time Synchronization** — Keep your development and operations data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GitLab Base URL and Personal Access Token (found in User Settings)
3. Start managing your projects from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Tech Leads** — quickly check the status of a merge request or list open issues without manual dashboard navigation.
- **Project Managers** — get a real-time overview of pipeline health and project activity via simple AI commands.
- **DevOps Engineers** — automate the retrieval of file contents and project metadata for auditing and automation.


## Available Tools (16)
- **verify_api_connection**: Check connection
- **create_project_issue**: Open an issue
- **get_repository_file**: Read file content
- **get_my_gitlab_profile**: Get user identity
- **create_merge_request**: Requires title.

Create a new merge request
- **get_merge_request**: Use the IID (the MR number shown in the UI, not the internal ID).

Get details for a specific merge request
- **list_branches**: List all branches in a project repository
- **list_project_members**: List all members of a project
- **get_project_details**: Get project metadata
- **list_visible_groups**: List accessible groups
- **list_project_issues**: List project issues
- **list_merge_requests**: List merge requests
- **list_project_pipelines**: List CI/CD pipelines
- **list_project_forks**: List forks
- **list_visible_projects**: List accessible projects
- **search_gitlab_global**: Search all GitLab


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitLab** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 open merge requests for project 'my-group/my-app'."

**🤖 AI Agent:**
> Retrieving merge requests... I found 5 recent open MRs, including 'Fix auth bug' and 'Add new dashboard'. Would you like the details for any of them?

---

**👤 You:**
> "Check the status of the latest pipelines for project ID '12345'."

**🤖 AI Agent:**
> Fetching pipelines... The latest pipeline for project 12345 'Success' 10 minutes ago. Previous pipeline 'Failed' due to a linting error.

---

**👤 You:**
> "Search GitLab for issues containing 'security patch'."

**🤖 AI Agent:**
> Searching issues... I found 3 issues matching 'security patch', including 'Patch for CVE-2024-001' in the 'Infra' project. Would you like to see the description?


## ❓ FAQ

**Q: How do I get a Personal Access Token (PAT) for GitLab?**
Log in to GitLab, go to User Settings > Access Tokens, and you can generate a new token with the 'api' scope there.

**Q: Does this support self-hosted GitLab instances?**
Yes! Simply provide your instance's root URL (e.g., https://gitlab.my-company.com) in the 'GitLab Base URL' credential field.

**Q: What is a 'Project ID' in GitLab?**
A Project ID is a unique numerical identifier for your project. You can also use the URL-encoded path (e.g., 'group%2Fproject') in most tools.

**Q: Can I see pipeline failures via the agent?**
Yes! Use the 'list_project_pipelines' tool to retrieve the status of all recent pipelines, allowing you to quickly identify failed builds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitlab](https://vinkius.com/mcp/gitlab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitLab** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitlab` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitLab** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitlab": {
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
