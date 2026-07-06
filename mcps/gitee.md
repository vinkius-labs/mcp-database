# Gitee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Collaborative code hosting and development platform — manage repositories, issues, and pull requests via AI.

## Description
Empower your AI agent to manage your development workflow on **Gitee**, the leading platform for collaborative software development in China. By connecting Gitee to your agent, you transform repository management and issue tracking into a natural conversation. Your agent can instantly list your repositories, create new issues, manage pull requests, and even read file contents without you needing to navigate the web interface. Whether you are a solo developer or part of a large team, your agent acts as a real-time development assistant, keeping your projects organized and moving forward.

### What you can do

- **Repository Management** — List all your repositories, get detailed info, and create new projects instantly.
- **Issue Tracking** — List, filter, and create issues to keep your tasks organized and track bugs efficiently.
- **Pull Requests** — Monitor and create pull requests to streamline your code review and merging process.
- **Code Access** — Retrieve file contents and directory structures to understand your codebase better.
- **Commit History** — Browse commit logs and audit changes across your branches and repositories.

### How it works

1. Subscribe to this server
2. Enter your Gitee Personal Access Token (PAT)
3. Start managing your projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — manage your Gitee projects and issues directly from your AI-powered workspace.
- **Project Managers** — track development progress, audit issues, and monitor pull requests through natural language.
- **Open Source Maintainers** — quickly respond to issues and oversee repository activity across multiple projects.
- **DevOps Teams** — integrate Gitee repository data into your automated workflows and AI-driven insights.


## Available Tools (10)
- **create_pull_request**: Create a pull request
- **create_repo**: Create a new repository
- **get_file_content**: Get file content
- **get_repo**: Get repository details
- **get_user**: Get authenticated user profile
- **list_repo_commits**: List repository commits
- **list_pull_requests**: List pull requests
- **list_repo_issues**: List repository issues
- **list_user_repos**: List authenticated user repositories
- **create_issue**: Create an issue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gitee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my repositories on Gitee."

**🤖 AI Agent:**
> I've retrieved your Gitee repositories. You have 5 active projects, including 'awesome-project' and 'demo-app'. Would you like more details on any of them?

---

**👤 You:**
> "Create a new issue in 'my-org/my-repo' titled 'Bug: login failure'."

**🤖 AI Agent:**
> Done! I've created issue #42 in the 'my-org/my-repo' repository with the title 'Bug: login failure'. You can track it here: [link].

---

**👤 You:**
> "Read the contents of README.md from the main branch of 'user/project'."

**🤖 AI Agent:**
> I've retrieved the README.md content for you. It contains project documentation, installation steps, and usage examples. Would you like me to summarize it?


## ❓ FAQ

**Q: How do I find my Gitee Personal Access Token?**
Log in to Gitee, go to [Settings -> Personal Access Tokens](https://gitee.com/profile/personal_access_tokens), and click 'Generate new token'. Make sure to copy it immediately as it won't be shown again.

**Q: Can I read the content of a file in a private repository?**
Yes, as long as your Personal Access Token has the necessary permissions (scopes) to access your private repositories, the `get_file_content` tool will work perfectly.

**Q: Is it possible to filter issues by their state?**
Yes. When using `list_repo_issues`, you can provide an optional `state` parameter (e.g., 'open', 'closed', or 'all') to filter the results according to your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitee](https://vinkius.com/mcp/gitee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gitee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gitee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitee": {
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
