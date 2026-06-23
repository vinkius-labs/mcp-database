# AccuLynx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acculynx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Business management for roofing contractors — manage leads, jobs, and financial data via AI.

## Description
Connect your **AccuLynx** account to your AI agent to streamline your roofing business operations. From creating new leads to auditing job milestones and payments, your agent manages your entire roofing workflow through natural conversation.

### What you can do

- **Lead Management** — Create and list leads to ensure your sales pipeline is always moving
- **Job Auditing** — Retrieve detailed information on active jobs, including milestones, insurance details, and assigned staff
- **Financial Monitoring** — Track payments, invoices, and accounting sync status across your projects
- **Contact Lookup** — Search for customer and user contact information quickly without leaving your chat
- **Document Oversight** — Audit job-related files and ensure all necessary documentation is in place for your roofing projects

### How it works

1. Subscribe to this server
2. Enter your AccuLynx API Key (generated via AppConnections)
3. Start managing your roofing jobs and leads through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Roofing Contractors** — manage jobs and leads more efficiently from the field or office
- **Sales Teams** — quickly add new leads and check project statuses on the fly
- **Operations Managers** — audit job progress and financial health across multiple locations
- **Accounting Staff** — monitor payment statuses and sync issues with ease


## Available Tools (4)
- **list_leads**: Retrieve a list of recent inquiries and prospective roofing projects in AccuLynx
- **create_lead**: Requires first and last name.

Add a prospective customer to the AccuLynx sales pipeline
- **get_job_details**: Requires a valid Job ID.

Retrieve technical milestones and metadata for a specific AccuLynx roofing job ID
- **list_payments**: Requires a valid Job ID.

Retrieve all payments and financial records associated with a specific AccuLynx job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AccuLynx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 leads created in my AccuLynx account."

**🤖 AI Agent:**
> I've retrieved your most recent leads. You have new inquiries from Smith, Johnson, and Brown families. Would you like to see the job details for any of them?


## ❓ FAQ

**Q: Where do I find my AccuLynx API Key?**
You must enable the **AppConnections** add-on in the AccuLynx Market (within your Account Settings). From there, you can generate unique API keys for each of your company locations.

**Q: Can I automate actions based on job status changes?**
Yes, AccuLynx allows you to configure webhooks to receive real-time notifications about job milestones, financial updates, or status changes.

**Q: Do I need developer skills to integrate?**
This MCP uses the custom REST API, so no extra code is needed on your end, but direct manual integrations would require API knowledge. Otherwise, AppConnections offers pre-built Zapier links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acculynx](https://vinkius.com/mcp/acculynx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AccuLynx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acculynx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AccuLynx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acculynx": {
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
