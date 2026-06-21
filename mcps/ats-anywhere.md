# ATS Anywhere MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ats-anywhere)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your recruiting process with ATS Anywhere — track jobs, applicants, and sites via AI.

## Description
The **ATS Anywhere MCP Server** (by HiringThing) provides a powerful natural language interface to your applicant tracking system. Empower your AI agent to manage your entire recruiting lifecycle, from job posting audits to applicant tracking and site management.

### Key Capabilities

- **Job Management** — List all job openings, retrieve detailed metadata for any specific position, and create new job listings directly from your chat.
- **Applicant Tracking** — Access your entire candidate database, including names, emails, and current application statuses.
- **Internal Notes** — Retrieve internal notes for any applicant to understand interviewer feedback and candidate history.
- **User Oversight** — List all recruiters and administrators associated with your ATS account.
- **Site Management** — Monitor all company sites and subdomains connected to your recruitment platform.
- **Secure API Access** — Uses secure HTTP Basic Authentication with your unique API Key and Password.

### Who is this for?

- **Recruiters** — Quickly audit active job listings and check applicant statuses without manual dashboard navigation.
- **Hiring Managers** — Review applicant details and internal notes using AI-assisted summaries during candidate evaluations.
- **Talent Acquisition Leads** — Monitor recruiting activity across multiple sites and teams using simple natural language.


## Available Tools
- **create_job**: Create a new job listing
- **get_account_check**: Verify ATS Anywhere account connection
- **get_applicant_notes**: Retrieve internal notes for an applicant
- **get_applicant**: Get full profile for a specific applicant
- **get_job**: Get details for a specific job
- **list_applicants**: List all job applicants
- **list_jobs**: List all job openings in ATS Anywhere
- **list_sites**: List all company sites/subdomains associated
- **list_users**: List all ATS users (recruiters/admins)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ATS Anywhere** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job openings in my ATS account."

**🤖 AI Agent:**
> I've retrieved your active jobs. You have 8 open positions, including 'Full Stack Developer', 'Marketing Lead', and 'Office Administrator'.

---

**👤 You:**
> "Show me the last 5 applicants received."

**🤖 AI Agent:**
> I've found the 5 most recent applicants. The latest is 'John Doe' who applied for the 'Full Stack Developer' role today.

---

**👤 You:**
> "Get internal notes for applicant ID 'app_12345'."

**🤖 AI Agent:**
> Retrieved 3 notes for applicant 'app_12345'. Highlights include positive feedback from the initial screening and a note about their availability starting next month.


## ❓ FAQ

**Q: How do I find my ATS Anywhere API Key and Password?**
Log in to your ATS dashboard, go to **Account Details**, scroll to the **Integrate** section, and select **API Access** to find your credentials.

**Q: Can I see recruiter notes for an applicant?**
Yes, use the `get_applicant_notes` tool and provide the Applicant ID to retrieve all internal notes and feedback associated with that candidate.

**Q: What is a 'Site' in ATS Anywhere?**
Sites are the individual instances or company subdomains configured in your HiringThing account. You can list them using the `list_sites` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ats-anywhere](https://vinkius.com/mcp/ats-anywhere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ATS Anywhere** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ats-anywhere` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ATS Anywhere** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ats-anywhere": {
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
