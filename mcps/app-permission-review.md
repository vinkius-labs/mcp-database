# App Permission Review MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/app-permission-review)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit application permissions against official requirements to identify security risks.

## Description
This MCP server provides a specialized auditing suite to compare user-supplied application permissions against a strict registry of approved permission sets. It helps identify privacy risks and compliance gaps by categorizing permissions into keep, review, or revoke statuses. Use `analyze_app_permissions` to perform a full audit, `get_app_requirements` to see the official permission list for an app, `list_all_apps` to see available applications, or `search_permission_by_name` to verify permission validity.


## Available Tools (4)
- **list_all_apps**: Provides a directory of all applications currently managed within the permission registry
- **get_app_requirements**: Retrieves the official list of approved permissions for a specific application
- **search_permission_by_name**: Checks if a specific permission string exists within the global domain context
- **analyze_app_permissions**: Performs the core audit of a specific application's permission profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **App Permission Review** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit the permissions for 'PhotoEditorApp' with permissions: ['camera', 'location', 'contacts']."

**🤖 AI Agent:**
> The audit for PhotoEditorApp is complete. Keep: ['camera']. Review: ['location', 'contacts']. The app is marked as unapproved due to the extra permissions requested.

---

**👤 You:**
> "What are the required permissions for 'WeatherService'?"

**🤖 AI Agent:**
> The required permissions for WeatherService are: ['location', 'network'].

---

**👤 You:**
> "Is 'biometric_auth' a valid permission?"

**🤖 AI Agent:**
> Yes, 'biometric_auth' is a recognized permission under the 'Security' category.


## ❓ FAQ

**Q: How do I audit a specific application?**
You can use the `analyze_app_permissions` tool by providing the application name and the list of permissions you want to check.

**Q: What does 'Review' status mean?**
A 'Review' status indicates that the application has requested a permission that is not found in its official required permission list, signaling a potential security risk.

**Q: Can I see all available apps in the registry?**
Yes, use the `list_all_apps` tool to retrieve a directory of all applications currently managed within the permission registry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/app-permission-review](https://vinkius.com/en/ai-agent-connect/app-permission-review)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **App Permission Review** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `app-permission-review` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **App Permission Review** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "app-permission-review": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
