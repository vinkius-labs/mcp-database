# Manatal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/manatal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manatal AI Recruitment and ATS platform to manage candidates, jobs, and applications.

## Description
Connect your **Manatal** account to any AI agent and take full control of your recruitment pipeline through natural conversation.

### What you can do

- **Candidate Management** — List all candidates, fetch detailed profiles, and manage your talent pool
- **Job Management** — Query active job openings, list departments, and manage career pages
- **Applications** — Track applicant progress and inspect individual application details
- **Client Management** — List and inspect organizations/clients associated with your recruitment firm

### How it works

1. Subscribe to this server
2. Enter your Manatal API Token
3. Start managing your recruitment process from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_application**: Get details for a specific application
- **get_candidate**: Get details for a specific candidate
- **get_job**: Get details for a specific job
- **get_organization**: Get details for a specific organization
- **list_applications**: List all applications
- **list_candidates**: List all candidates
- **list_career_pages**: List all career pages
- **list_departments**: List all departments
- **list_jobs**: List all jobs
- **list_organizations**: List all organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Manatal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first page of candidates."

**🤖 AI Agent:**
> Fetching candidates... I found several candidates including John Doe and Jane Smith. Would you like to see more details for any of them?

---

**👤 You:**
> "What are the active job openings?"

**🤖 AI Agent:**
> Querying job openings... There are currently 5 active jobs, such as 'Senior Developer' and 'Product Manager'.

---

**👤 You:**
> "Get details for organization ID 123."

**🤖 AI Agent:**
> Inspecting organization... Organization 123 is 'TechCorp Inc.', with 10 active job openings.


## ❓ FAQ

**Q: Where can I find my Manatal API Token?**
Log in to Manatal, go to Administration > Integration > API, and you will find your API Token there.

**Q: Can I list candidates by page?**
Yes, use the `list_candidates` tool and provide the `page` parameter to navigate through your results.

**Q: Is my data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manatal](https://vinkius.com/mcp/manatal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Manatal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `manatal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Manatal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "manatal": {
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
