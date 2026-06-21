# ApplicantStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/applicantstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your hiring process with ApplicantStack — track jobs, candidates, and hires via AI.

## Description
The **ApplicantStack MCP Server** integrates your recruiting and onboarding workflows directly into your AI workspace. Efficiently manage your job listings, track candidate progress through custom stages, and streamline your hiring process using simple natural language.

### Key Features

- **Job Management** — List all active and closed job openings, and retrieve full metadata for any specific listing.
- **Candidate Tracking** — Access your entire applicant database and filter by workflow stage or score.
- **Workflow Automation** — Move candidates between stages (e.g., from 'Interview' to 'Hired') and update their profiles instantly.
- **Onboarding & Hires** — Access onboarding data for new hires to ensure a smooth transition from applicant to employee.
- **Secure Access** — Uses private access tokens to safely interact with your organization's recruiting data.

### Benefits for Teams

- **Recruiters** — Quickly check the status of candidates for multiple jobs without switching between tabs.
- **Hiring Managers** — Review candidate profiles and scores using AI-assisted summaries.
- **HR Teams** — Track hiring trends and ensure onboarding tasks are initiated for all new hires.


## Available Tools
- **get_account_check**: Verify ApplicantStack account connection
- **get_candidate**: Get details for a specific candidate
- **get_job**: Get details for a specific job
- **list_candidates**: List all candidates
- **list_hires**: List all hires (onboarding)
- **list_jobs**: List all job listings in ApplicantStack
- **update_candidate**: Use stage field to move them in the workflow.

Update candidate information or stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ApplicantStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job openings in ApplicantStack."

**🤖 AI Agent:**
> I've retrieved your active jobs. You have 5 open positions, including 'Software Engineer', 'Product Designer', and 'HR Manager'.

---

**👤 You:**
> "Show me candidates currently in the 'Interview' stage."

**🤖 AI Agent:**
> There are 3 candidates currently in the Interview stage: John Doe, Jane Smith, and Alex Johnson.

---

**👤 You:**
> "Move candidate 'C12345' to the 'Hired' stage."

**🤖 AI Agent:**
> Candidate 'C12345' has been successfully moved to the 'Hired' stage.


## ❓ FAQ

**Q: How do I find my ApplicantStack API Token?**
Log in to ApplicantStack, go to **Settings**, then **Edit Settings**. Your API token will be listed under the API section.

**Q: What is the subdomain?**
The subdomain is the first part of your ApplicantStack URL (e.g., if your URL is `mycompany.applicantstack.com`, your subdomain is `mycompany`).

**Q: Can I move a candidate to a new stage?**
Yes, use the `update_candidate` tool and provide the new stage name in the `stage` field to advance them in your workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/applicantstack](https://vinkius.com/mcp/applicantstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ApplicantStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `applicantstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ApplicantStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "applicantstack": {
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
