# Codacy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/codacy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage code quality and automated reviews via Codacy — track grades, monitor issues, and audit repository analysis directly from any AI agent.

## Description
Connect your **Codacy** account to any AI agent and take full control of your automated code reviews and quality metrics through natural conversation. Streamline how you monitor security and maintainability across your repositories natively.

### What you can do

- **Organization Oversight** — List and retrieve details for all organizations associated with your Codacy account natively
- **Repository Intelligence** — Access current quality grades, complex files, and overall metrics for any analyzed repository flawlessly
- **Issue Management** — Search for specific code quality issues using advanced filters like level, category, and language securely
- **Language Logistics** — List all programming languages supported by the Codacy analysis engine flawlessly
- **Member Management** — Access organization member rosters and user profile information securely
- **Webhook Visibility** — Monitor configured webhooks for real-time quality and analysis notifications directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Codacy Account API Token (found in User Settings > API)
3. Start managing your code quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Managers** — monitor repository grades and quality trends using natural language
- **DevOps Engineers** — audit repository webhooks and analysis status without opening the dashboard
- **Software Developers** — quickly look up specific code issues and security alerts straight from their chat interface
- **Security Teams** — verify repository compliance and monitor vulnerability findings


## Available Tools (8)
- **get_repository_quality_analysis**: Get the current quality grade and metrics for a specific repository
- **list_supported_languages**: List programming languages supported by the Codacy analysis engine
- **get_my_codacy_profile**: Retrieve information about the authenticated Codacy user
- **list_codacy_organizations**: List all organizations associated with the account
- **list_organization_members**: List people and users belonging to an organization
- **list_organization_repositories**: List all repositories analyzed within an organization
- **list_repository_webhooks**: List configured webhooks for quality notifications
- **search_repository_issues**: Search for specific code quality issues in a repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Codacy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all repositories in the 'vinkius' organization on GitHub."

**🤖 AI Agent:**
> Retrieving repositories for gh/vinkius... I found 5 analyzed repositories: 'core-api' (Grade: A), 'web-frontend' (Grade: B), 'mcp-servers' (Grade: A), and 2 others. Which one would you like to see issues for?

---

**👤 You:**
> "Show me the security issues for the 'core-api' repository."

**🤖 AI Agent:**
> Searching for security issues in gh/vinkius/core-api... I found 2 'Critical' security vulnerabilities related to SQL injection patterns and 1 'Medium' warning about hardcoded secrets.

---

**👤 You:**
> "What languages does Codacy support?"

**🤖 AI Agent:**
> Retrieving supported languages... Codacy supports over 40 languages including JavaScript, TypeScript, Python, Go, Java, PHP, Ruby, and C#. It also supports configuration files like Dockerfile and Terraform.


## ❓ FAQ

**Q: Can I see the quality grade for a specific repository?**
Yes! Use the `get_repository_quality_analysis` tool. Provide the provider (e.g., `gh`), organization, and repository name. The agent will return the current letter grade (A-F) and core quality metrics.

**Q: How do I search for security-related issues in my code?**
Use the `search_repository_issues` tool. You can filter the payload to include `categories: ['Security']`. Your agent will fetch all security vulnerabilities identified by Codacy in that repository.

**Q: Where do I find my Codacy API Token?**
Log in to Codacy, click on your avatar in the top right, go to **User Settings**, and select the **API** tab. You can generate and copy your account token from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codacy](https://vinkius.com/mcp/codacy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Codacy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `codacy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Codacy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "codacy": {
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
