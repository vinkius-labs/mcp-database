# UKG Pro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ukg-pro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage HR data, employee profiles, and payroll via UKG Pro.

## Description
The UKG Pro MCP Server integrates the Model Context Protocol with the UKG Pro human capital management suite, enabling AI agents to manage HR data, employee profiles, payroll details, and organizational structures seamlessly.


## Available Tools
- **organizations**: List organizational components and structures
- **employees**: Get a specific employee by ID in UKG Pro
- **jobs**: Get a specific job configuration by job code
- **payroll**: Get payroll records for the current pay period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UKG Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the contact details for employee ID 12345."

**🤖 AI Agent:**
> Here are the contact details for employee 12345: John Doe, Email: john.doe@example.com...

---

**👤 You:**
> "Show the current organizational reporting structure for the 'Marketing' division."

**🤖 AI Agent:**
> Querying UKG Pro organization charts ('get_org_metrics')...
Marketing Division hierarchy:
- VP of Marketing: Sarah Jenkins
  |- Director of Content: Mark D.
  |- Director of SEO: Alice R.
Total active headcounts beneath VP: 45.

---

**👤 You:**
> "Verify the payroll status for the latest bi-weekly run."

**🤖 AI Agent:**
> Fetching payroll parameters ('get_payroll_status')...
The bi-weekly run (Pay Period: Oct 1 - Oct 15) is 'Completed'. Direct deposits were dispatched successfully on Oct 17. Gross payroll total: $450,210.


## ❓ FAQ

**Q: What data can be accessed via the UKG Pro MCP Server?**
You can access employee profiles, compensation details, job history, payroll information, user details, and organizational structures.

**Q: What authentication methods are supported?**
The server supports API Keys/Service Account Basic Authentication and OAuth2 depending on your UKG Pro environment endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ukg-pro](https://vinkius.com/mcp/ukg-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UKG Pro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ukg-pro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UKG Pro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ukg-pro": {
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
