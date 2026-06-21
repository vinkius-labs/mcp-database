# UKG Pro Learning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ukg-pro-learning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage employee training, courses, and learning paths via UKG Pro Learning.

## Description
The UKG Pro Learning MCP Server integrates the Model Context Protocol with the UKG LMS, enabling AI agents to query training catalogs, track employee course completions, manage learning paths, and fetch enrollment data.


## Available Tools
- **enrollments**: List enrollments for a specific user
- **courses**: Get a specific training course by ID
- **curricula**: List tracking curricula (Learning Paths)
- **users**: Get details for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UKG Pro Learning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active training courses available to the Sales team."

**🤖 AI Agent:**
> Here are the active courses for the Sales team: 1) Advanced Negotiation Skills, 2) Sales Process Overview...

---

**👤 You:**
> "Check the training completion status for employee 'Jane Smith' on the compliance path."

**🤖 AI Agent:**
> Querying UKG Learning records ('get_user_progress')...
Jane Smith (ID: 8841) has completed 80% of the '2026 Annual Compliance' path. 
Remaining modules: 'Data Privacy Basics'.

---

**👤 You:**
> "Assign the 'Cybersecurity 101' curriculum to all new hires in the Engineering department."

**🤖 AI Agent:**
> Executing `assign_curriculum`... Successfully enrolled 12 new Engineering hires into 'Cybersecurity 101' (Curriculum ID: 4022). Due date set for 30 days from today.


## ❓ FAQ

**Q: What learning data can AI agents manage?**
Agents can access training courses, curricula, learning paths, employee enrollments, and completion records.

**Q: How is authentication handled for UKG Pro Learning?**
Authentication relies on an API key or an OAuth2 access token provided by your UKG Pro Learning / Schoox environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ukg-pro-learning](https://vinkius.com/mcp/ukg-pro-learning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UKG Pro Learning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ukg-pro-learning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UKG Pro Learning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ukg-pro-learning": {
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
