# Illumidesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/illumidesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage campuses, courses, and users via Illumidesk LMS API.

## Description
Connect your AI agents to Illumidesk, the AI-powered learning management system. This MCP server allows you to list campuses, manage courses, track user memberships, and access activity logs directly through the Illumidesk API. Ideal for automating education workflows and course management.


## Available Tools (10)
- **get_activity_logs**: Retrieves activity logs for a specific campus
- **get_campus**: Retrieves details for a specific campus
- **get_course**: Retrieves details for a specific course
- **get_me**: Gets current authenticated user info
- **list_campuses**: Lists all campuses in Illumidesk
- **list_courses**: Lists all courses within a specific campus
- **list_lti_credentials**: Lists all LTI credentials for a campus
- **list_lti_deployments**: Lists all LTI deployments for a campus
- **list_memberships**: Lists all user memberships in a specific campus
- **list_users**: Lists all users registered in a specific campus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Illumidesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all campuses in my Illumidesk account."

**🤖 AI Agent:**
> I'll fetch the list of your Illumidesk campuses.

---

**👤 You:**
> "Show me courses for campus slug 'main-campus'."

**🤖 AI Agent:**
> I'll retrieve the list of courses for that specific campus.

---

**👤 You:**
> "Check who is enrolled in course 'ai-fundamentals'."

**🤖 AI Agent:**
> I'll look up the user memberships for that course.


## ❓ FAQ

**Q: How do I get Illumidesk API credentials?**
You can find your API key in your Illumidesk account settings under the 'Developer' or 'Integrations' section.

**Q: What is a campus slug?**
A slug is a unique identifier for your campus or course, usually found in the URL (e.g., app.illumidesk.com/campus/my-campus-slug/).

**Q: Does it support LTI integrations?**
Yes, you can list LTI credentials and deployments using the dedicated tools in this MCP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/illumidesk](https://vinkius.com/mcp/illumidesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Illumidesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `illumidesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Illumidesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "illumidesk": {
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
