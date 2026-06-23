# Forgejo (Gitea Fork) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/forgejo-gitea-fork)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Forgejo and Gitea instances — check version compatibility, generate API tokens, and trigger CI/CD workflows directly from your AI agent.

## Description
Connect your **Forgejo** or **Gitea** instance to any AI agent to streamline your DevOps and repository management workflows through natural conversation.

### What you can do

- **Version Auditing** — Retrieve detailed Forgejo and Gitea-compatible version information to ensure API compatibility across your infrastructure.
- **Token Management** — Generate new Personal Access Tokens (PATs) with specific scopes (read/write) using your BasicAuth credentials.
- **CI/CD Automation** — Trigger manual workflow dispatches for Forgejo Actions directly from the chat to start builds or deployments.
- **Instance Inspection** — Verify the health and configuration of your self-hosted Git service without leaving your development environment.

### How it works

1. Subscribe to this server
2. Enter your Forgejo Instance URL and credentials (Token or Username/Password)
3. Start managing your repositories and actions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the triggering of CI/CD pipelines and monitor instance versions across multiple environments.
- **Software Developers** — generate API tokens for local scripts or integrations without navigating the web UI.
- **System Administrators** — quickly audit self-hosted Git instances and manage access credentials via AI assistance.


## Available Tools (4)
- **create_token**: Generates a new personal access token.

Generate a new API token for a user
- **dispatch_workflow**: Trigger a manual workflow dispatch in Forgejo Actions
- **get_forgejo_version**: Get detailed Forgejo version information
- **get_gitea_version**: Get the Gitea-compatible version of the Forgejo instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forgejo (Gitea Fork)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the Forgejo and Gitea-compatible versions of my instance."

**🤖 AI Agent:**
> I've checked your instance. It is running Forgejo version 7.0.1 and is compatible with Gitea API version 1.21.0.

---

**👤 You:**
> "Generate a new API token named 'CI-Runner' with read:repository scope for user 'admin'."

**🤖 AI Agent:**
> I have successfully created the token 'CI-Runner' for user 'admin'. The token is: [TOKEN_VALUE]. Please save it securely.

---

**👤 You:**
> "Trigger the 'deploy.yaml' workflow in the 'main-app' repository owned by 'dev-team'."

**🤖 AI Agent:**
> The workflow 'deploy.yaml' has been successfully dispatched for dev-team/main-app. You can monitor the progress in your Forgejo Actions dashboard.


## ❓ FAQ

**Q: How can I check which Forgejo version my instance is running?**
You can use the `get_forgejo_version` tool. It will return the specific version string of your Forgejo instance, which is useful for debugging and feature compatibility checks.

**Q: Can I trigger a CI/CD build manually through the AI?**
Yes! Use the `dispatch_workflow` tool by providing the repository owner, name, and the workflow file name. This triggers actions configured with the 'workflow_dispatch' event.

**Q: What is required to generate a new API token?**
To use the `create_token` tool, you must have your Forgejo username and password configured in the credentials. This allows the agent to authenticate via BasicAuth and request a new token with your specified scopes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forgejo-gitea-fork](https://vinkius.com/mcp/forgejo-gitea-fork)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Forgejo (Gitea Fork)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `forgejo-gitea-fork` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Forgejo (Gitea Fork)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "forgejo-gitea-fork": {
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
