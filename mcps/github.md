# GitHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/github)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage repositories, track issues, and search code via AI agents with GitHub.

## Description
Connect your **GitHub** account to any AI agent to automate your software development lifecycle and code management through the Model Context Protocol (MCP). GitHub is the world's leading AI-powered developer platform. This MCP server enables you to retrieve repository metadata, manage issues, track pull requests, and search for code directly through natural conversation.

### Key Features

- **Repository Oversight** — List all repositories for any user or organization, and fetch detailed configuration metadata for specific projects.
- **Issue & PR Management** — List issues and pull requests, track their lifecycle status, and programmatically open new issues from your chat interface.
- **Code Content Discovery** — Retrieve the contents of files or directories within any repository to understand codebase structures.
- **Advanced Code Search** — Execute powerful searches across GitHub's massive database to isolate specific code snippets or repositories.
- **Collaboration Tracking** — Monitor forks and contributors to understand project community engagement.
- **Identity Oversight** — Access detailed profile information for the authenticated GitHub user to verify permissions and account context.
- **Real-time Synchronization** — Keep your source control and development data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GitHub Personal Access Token (found in Settings > Developer settings)
3. Start managing your repositories from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Tech Leads** — quickly check the status of a pull request or list open issues without manual dashboard navigation.
- **Project Managers** — get a real-time overview of repository activity and community engagement via simple AI commands.
- **DevOps Engineers** — automate the retrieval of file contents and repository metadata for auditing and workflows.


## Available Tools (18)
- **verify_api_connection**: Check connection
- **list_user_repositories**: List user repos
- **create_pull_request**: Requires the head branch (your changes) and base branch (merge target).

Create a pull request
- **add_issue_comment**: Supports markdown formatting.

Add a comment to an issue or PR
- **create_new_issue**: Open an issue
- **get_file_contents**: Read file content
- **get_issue_details**: Get a specific issue by number
- **get_my_github_profile**: Get user identity
- **get_repository_details**: Get repo metadata
- **list_branches**: List repository branches
- **list_commits**: Optionally filter by branch name or SHA.

List recent commits
- **list_repo_issues**: List repo issues
- **list_org_repositories**: List organization repositories
- **list_pull_requests**: List pull requests
- **list_releases**: List repository releases
- **list_stargazers**: Useful for popularity tracking.

List repository stargazers
- **search_github_code**: Search code snippets
- **search_github_repositories**: Search all repos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 open issues in the 'facebook/react' repository."

**🤖 AI Agent:**
> Retrieving issues... I found 5 recent open issues in react, including 'Bug: Hydration error' and 'Feature request: New hook'. Would you like the details for any of them?

---

**👤 You:**
> "Find all repositories for the organization 'vinkius'."

**🤖 AI Agent:**
> Searching organization... I found 12 repositories for Vinkius, including 'vurb-core' and 'mcp-originals'. Would you like to see the stars count for these?

---

**👤 You:**
> "Read the content of the 'README.md' file in 'vinkius/vurb-docs'."

**🤖 AI Agent:**
> Fetching file... The README.md for vurb-docs contains: '# Vurb Documentation - Welcome to the official guide...'. Would you like me to summarize the installation steps?


## ❓ FAQ

**Q: How do I get a Personal Access Token (PAT) for GitHub?**
Log in to GitHub, go to Settings > Developer settings > Personal access tokens, and you can generate a new token (classic or fine-grained) there.

**Q: Can I read private repositories?**
Yes, provided that your Personal Access Token has the necessary scopes (e.g., 'repo') to access your private content.

**Q: How do I search for code within a specific organization?**
Use the 'search_github_code' tool and include the organization qualifier in your query, for example: 'org:vinkius my-term'.

**Q: Can I comment on issues via the agent?**
Yes! Use the `add_issue_comment` tool — provide the repository owner, name, and the issue or PR number along with your comment text (markdown supported). Your agent will post the comment instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github](https://vinkius.com/mcp/github)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `github` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "github": {
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
