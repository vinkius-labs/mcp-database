# Innform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/innform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage learners, courses, and results via Innform LMS API.

## Description
Empower your AI agents to manage your training platform with Innform. This MCP server allows you to list learners, track course completion, manage learning pathways, and view results directly through the Innform API. Ideal for automating corporate training and employee development.


## Available Tools
- **get_learner**: Retrieves details for a specific learner
- **get_me**: Gets current authenticated user info
- **list_courses**: Lists all courses
- **list_departments**: Lists all departments
- **list_learners**: Lists all learners in Innform
- **list_locations**: Lists all organization locations
- **list_modules**: Lists all training modules
- **list_pathways**: Lists all learning pathways
- **list_results**: Lists learner assessment and course results
- **list_tags**: Lists all defined tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Innform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active learners in my Innform account."

**🤖 AI Agent:**
> I'll fetch the list of your active learners.

---

**👤 You:**
> "Show me the results for 'Cybersecurity Awareness' course."

**🤖 AI Agent:**
> I'll retrieve the learner results for that specific course.

---

**👤 You:**
> "Check for any new learning pathways."

**🤖 AI Agent:**
> I'll look up the list of available learning pathways in Innform.


## ❓ FAQ

**Q: How do I get Innform API credentials?**
You can generate an API key in your Innform account under Account Settings > API. Ensure you have the necessary permissions.

**Q: Can I see learner results?**
Yes, the list_results tool provides access to assessment and course completion data for your learners.

**Q: Are learning pathways supported?**
Yes, you can list all defined learning pathways using the list_pathways tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/innform](https://vinkius.com/mcp/innform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Innform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `innform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Innform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "innform": {
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
