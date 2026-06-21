# Liaison MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liaison)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Centralize admissions and enrollment management for higher education with applicant tracking and document collection workflows.

## Description
Connect your **Liaison WebAdMIT** account to any AI agent and manage admissions operations.

### What you can do

- **Application Management** — List and inspect applications with full details
- **Export Management** — View and download data exports
- **Batch Processing** — List and review application batches
- **Program Administration** — Browse academic programs
- **Schema Access** — View designations and custom field definitions


## Available Tools (11)
- **check_liaison_status**: Verify API connectivity
- **get_application**: Get application details
- **get_batch**: Get batch details
- **get_export**: Get export details
- **get_program**: Get program details
- **list_applications**: List all applications
- **list_batches**: List application batches
- **list_custom_fields**: List custom fields
- **list_designations**: List designations
- **list_exports**: List data exports
- **list_programs**: List academic programs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liaison** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending applications."

**🤖 AI Agent:**
> You have 342 applications: 128 under review, 89 pending documents, 78 complete, 47 awaiting decision.

---

**👤 You:**
> "Show details for application app_2891."

**🤖 AI Agent:**
> Application app_2891: Jane Doe, Applied to 'MBA Program', submitted 2024-03-15, status: Under Review. GPA: 3.8, GMAT: 720.

---

**👤 You:**
> "List all academic programs."

**🤖 AI Agent:**
> 8 programs: MBA (234 applicants), MS Computer Science (189), MS Data Science (156), JD Law (98).


## ❓ FAQ

**Q: Can my AI browse admissions applications?**
Yes. `list_applications` returns all applications and `get_application` shows full details for any one.

**Q: Can I access data exports?**
Yes. `list_exports` and `get_export` let you find and download configured data exports.

**Q: How do I view academic programs?**
`list_programs` shows all programs and `get_program` returns full details including requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liaison](https://vinkius.com/mcp/liaison)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liaison** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liaison` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liaison** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liaison": {
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
