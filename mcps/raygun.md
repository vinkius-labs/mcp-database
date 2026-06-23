# Raygun MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/raygun)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor application health, track deployments, and manage crash reports and RUM sessions directly from your AI agent.

## Description
Connect your **Raygun** account to any AI agent to gain deep visibility into your application's performance and stability through natural language.

### What you can do

- **Application Management** — List all accessible applications and environments within your Raygun account.
- **Deployment Tracking** — Monitor and list deployments for specific applications to correlate releases with performance changes.
- **Crash Reporting** — Manually send crash reports and error payloads to the Raygun API for centralized tracking.
- **Real User Monitoring (RUM)** — Authenticate and search through user sessions to understand real-world performance and user journeys.
- **Session Inspection** — Retrieve detailed metadata for specific RUM sessions to debug user-specific issues.

### How it works

1. Subscribe to this server
2. Enter your Raygun Personal Access Token (PAT) or API Key
3. Start monitoring your stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — Quickly check deployment history and application health without leaving the terminal or chat.
- **Software Engineers** — Send manual crash reports during testing or inspect RUM sessions to reproduce bugs.
- **Product Owners** — Query user session data to understand how new features are performing in the wild.


## Available Tools (7)
- **create_legacy_deployment**: Create a deployment using the legacy API
- **list_applications**: List accessible Raygun applications
- **list_deployments**: List deployments for a specific application
- **rum_authenticate**: Authenticate with the legacy RUM API
- **rum_get_session**: Get RUM session details
- **rum_search_sessions**: Search RUM sessions
- **send_crash_report**: Send a manual crash report to Raygun


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Raygun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Raygun applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 'Main-Web-App' (ID: abc-123) and 'Mobile-API' (ID: def-456) active. Which one would you like to inspect?

---

**👤 You:**
> "Show me the latest deployments for application ID abc-123."

**🤖 AI Agent:**
> Fetching deployments for 'Main-Web-App'... I found 3 recent deployments. The latest was version 2.1.0, deployed 2 hours ago by 'CI-Runner'.

---

**👤 You:**
> "Search for RUM sessions from the US using session key XYZ."

**🤖 AI Agent:**
> Searching RUM sessions... I found 12 sessions from the US. Most users are on Chrome/macOS. Would you like to see the details for the most recent session?


## ❓ FAQ

**Q: How can I see a list of all my Raygun applications?**
Use the `list_applications` tool. It will retrieve all applications associated with your Personal Access Token, including their IDs and names.

**Q: Can I manually report an error that happened on a specific machine?**
Yes, use the `send_crash_report` tool. You can specify the machine name, error message, stack trace, and even custom data to be sent to Raygun.

**Q: How do I search for user sessions from a specific country?**
First, authenticate using `rum_authenticate` to get a session key. Then, use `rum_search_sessions` and provide the country code in the parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/raygun](https://vinkius.com/mcp/raygun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Raygun** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `raygun` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Raygun** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "raygun": {
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
