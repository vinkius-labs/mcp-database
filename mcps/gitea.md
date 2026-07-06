# Gitea MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitea)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage self-hosted Git via Gitea — list and manage repositories, track issues and pull requests, handle organizations, and audit branches directly from any AI agent.

## Description
Connect your **Gitea** instance to any AI agent and take full control of your self-hosted Git services, code reviews, and project collaboration through natural conversation.

### What you can do

- **Repository Orchestration** — List all accessible repositories and retrieve full details including descriptions, clone URLs, stars, and visibility states natively
- **Issue & Task Tracking** — Enumerate issues in any repository to track numbers, states, labels, and assignees, and retrieve full body content for detailed analysis flawlessly
- **Pull Request Auditing** — List all pull requests to monitor open, closed, or merged states and review source/target branch mappings synchronously
- **Organization Management** — Identify organizations you belong to and retrieve detailed org metadata including website, location, and repository counts securely
- **Branch & Protection Oversight** — List all branches in a repository and verify commit SHAs and effective branch protection rules natively
- **User Profile Discovery** — Extract the authenticated profile identity including login, email, full name, and administrative status flawlessy
- **Project Navigation** — Analyze specific localized variables decoding active data routes and extracting hidden structural constraints within your Gitea environment

### How it works

1. Subscribe to this server
2. Enter your Gitea Instance URL and Access Token (found in your Gitea User Settings > Applications)
3. Start managing your code from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers & Engineering Leads** — track pull requests and manage repository issues without leaving the chat or IDE interface
- **Indie Hackers & Self-Hosters** — monitor your private Gitea instance and verify repository statuses using natural language
- **Product Managers** — audit project issues and organization structures to analyze team progress in real-time
- **DevOps Engineers** — test and debug Git API integrations and verify branch protection rules through natural conversation


## Available Tools (10)
- **get_repo**: Get full details of a Gitea repository
- **list_issues**: List all issues in a Gitea repository
- **get_issue**: Get full details of a Gitea issue
- **list_orgs**: List all organizations the authenticated Gitea user belongs to
- **get_org**: Get full details of a Gitea organization
- **list_org_repos**: List all repositories belonging to a Gitea organization
- **list_pulls**: List all pull requests in a Gitea repository
- **list_branches**: List all branches in a Gitea repository
- **get_me**: Get the authenticated Gitea user profile
- **list_repos**: Returns repo full names, descriptions, clone URLs, stars, forks, private/public status, and default branches.

List all repositories accessible to the authenticated Gitea user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gitea** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 repositories I worked on"

**🤖 AI Agent:**
> Retrieving your repositories... I found 5 recent projects including 'web-app', 'api-service', and 'infra-config'. Highlights: 'web-app' (Default: main, Visibility: private). Which one would you like to see the issues for?

---

**👤 You:**
> "Show me open pull requests for repo 'api-service'"

**🤖 AI Agent:**
> Retrieving PRs for 'api-service'... I found 2 open pull requests: #101 'Add OAuth support' and #102 'Fix rate-limiting bug'. Would you like the review status or branch details for either of these?

---

**👤 You:**
> "List all issues in organization 'Eng-Team'"

**🤖 AI Agent:**
> Retrieving organization issues... I found 15 issues across the 'Eng-Team' repositories. Most are in 'core-engine' and 'frontend-v2'. Would you like me to filter them by labels or assignees?


## ❓ FAQ

**Q: Can my agent list all issues in a Gitea repository?**
Yes. Use the 'list_issues' tool. Provide the owner and repository name. The agent will return all issues with their titles, numbers, states, and labels, allowing you to monitor project progress natively.

**Q: How do I check the details of a specific pull request via chat?**
Use the 'list_pulls' tool to see active PRs and their numbers. You can then ask for details about a specific PR to verify source/target branches and current review status synchronously.

**Q: Can I see all repositories belonging to a Gitea organization through the agent?**
Absolutely. Use the 'list_org_repos' tool. Provide the organization name, and the agent will return all repositories belonging to that org, including their clone URLs and visibility status natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitea](https://vinkius.com/mcp/gitea)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gitea** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitea` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gitea** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitea": {
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
