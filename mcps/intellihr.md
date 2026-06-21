# intelliHR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/intellihr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee directory, jobs, and organization data via intelliHR API.

## Description
Connect your AI agents to intelliHR, the strategic people management platform. This MCP server allows you to list and retrieve employee profiles, track job assignments, manage positions and business entities, and view organization data directly through the intelliHR API. Ideal for automating HR operations and employee data analysis.


## Available Tools
- **get_person**: Retrieves details for a specific person
- **list_business_entities**: Lists all legal business entities
- **list_jobs**: Lists all jobs/positions currently assigned
- **list_locations**: Lists all registered office locations
- **list_people**: Lists all people/employees in intelliHR
- **list_positions**: Lists all defined position titles
- **list_remuneration**: Lists employee remuneration and pay details
- **list_skills**: Lists all skills defined in the organization
- **list_training**: Lists all employee training and development records
- **list_users**: Lists all users with platform access


## 💬 Prompt Examples

Here are some examples of how you can interact with the **intelliHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the intelliHR directory."

**🤖 AI Agent:**
> I'll fetch the complete employee directory for you.

---

**👤 You:**
> "Show me details for employee ID '123'."

**🤖 AI Agent:**
> I'll retrieve the full profile and job history for that specific employee.

---

**👤 You:**
> "List all registered office locations."

**🤖 AI Agent:**
> I'll look up the list of office locations in your organisation.


## ❓ FAQ

**Q: How do I get intelliHR API credentials?**
Log in to your intelliHR platform, navigate to Settings > Public API Access Keys, and create a new access key. Note that the key is only displayed once.

**Q: What is the 'tenant'?**
The tenant is your organisation's unique identifier in intelliHR, usually the subdomain of your login URL (e.g., if you log in at acme.intellihr.net, your tenant is 'acme').

**Q: Are sensitive fields like remuneration supported?**
Yes, the list_remuneration tool provides access to remuneration data, provided your API Access Key has the necessary system administrator permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intellihr](https://vinkius.com/mcp/intellihr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **intelliHR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `intellihr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **intelliHR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intellihr": {
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
