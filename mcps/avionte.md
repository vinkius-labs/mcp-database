# Avionte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avionte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage staffing and recruiting workflows via Avionte — query talent profiles, work history, company details, and department data directly from your AI agent.

## Description
Connect your **Avionte** staffing platform to any AI agent and streamline your recruitment and talent management workflows through natural conversation.

### What you can do

- **Talent Management** — Retrieve comprehensive talent profiles, including work history, education records, and current nomination stages.
- **Company & Department Insights** — Fetch detailed information about companies, specific departments, and their physical addresses.
- **Payroll & Banking** — Securely access talent direct deposit account information and banking details for administrative tasks.
- **Workflow Tracking** — Monitor talent tags, available statuses, and company-specific purchase orders (POs) to keep your staffing operations organized.
- **Data Categorization** — List and manage tags for both talent and companies to ensure precise filtering and reporting.

### How it works

1. Subscribe to this server
2. Enter your Avionte API Key, Client ID, Client Secret, and Tenant ID
3. Start managing your staffing pipeline from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated recruiting coordinator, providing instant access to candidate data and organizational structures without switching between multiple software modules.

### Who is this for?

- **Recruiters & Sourcers** — quickly pull candidate backgrounds and check nomination stages during the screening process.
- **HR Operations** — verify banking details and education history for onboarding without manual data entry.
- **Account Managers** — retrieve company tags and department structures to better serve client staffing needs.


## Available Tools (16)
- **get_company_restrictions**: Get talent restrictions for a company
- **get_company_tags**: Get tags for a company
- **get_company**: Retrieve company details
- **get_department_address**: Get a specific department address
- **get_department**: Retrieve department details
- **get_job**: Retrieve job details
- **get_multiple_pipeline_by_pipeline_ids**: Get details for multiple job pipelines
- **get_talent_direct_deposit_accounts**: Get direct deposit accounts for a talent
- **get_talent_education_history**: Retrieve education history for a talent
- **get_talent_stage**: Get details about a talent nomination stage
- **get_talent**: Provide talentId or other query parameters as needed.

Retrieve details for a specific talent
- **get_talent_work_history**: Retrieve work history for a talent
- **get_web_applications_for_talent**: List jobs a talent has applied for
- **get_all_talent_tags**: Get all tags associated with a talent
- **get_available_talent_statuses**: List all available talent statuses
- **get_company_po_by_po_id**: Retrieve a specific purchase order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Avionte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the full profile and work history for talent ID 98765."

**🤖 AI Agent:**
> I've fetched the data for talent 98765. The candidate is Jane Smith. Her work history includes 3 years as a Senior Developer at TechCorp and 2 years at WebSolutions. Would you like to see her education history as well?

---

**👤 You:**
> "What is the current nomination stage for talent 12345?"

**🤖 AI Agent:**
> Talent 12345 is currently in the 'Final Interview' stage of the nomination process. The next step scheduled is 'Reference Check'.

---

**👤 You:**
> "Get the address for department ID 5544 and list any tags for company ID 100."

**🤖 AI Agent:**
> Department 5544 is located at 123 Innovation Way, Suite 400. For company 100, I found the following tags: 'Strategic Partner', 'High Volume', and 'IT Services'.


## ❓ FAQ

**Q: Can I see a candidate's full work and education history using their ID?**
Yes! You can use the `get_talent_work_history` and `get_talent_education_history` tools with the specific Talent ID to retrieve all recorded employment and academic background details.

**Q: How do I check the current nomination stage of a talent in the hiring process?**
Simply use the `get_talent_stage` tool. It will return the specific stage of the nomination process for the provided Talent ID, helping you track where they are in the pipeline.

**Q: Is it possible to list all available talent statuses configured in our system?**
Yes, the `get_available_talent_statuses` tool retrieves a complete list of all possible statuses that can be assigned to talent profiles within your Avionte environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avionte](https://vinkius.com/mcp/avionte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Avionte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `avionte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Avionte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "avionte": {
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
