# Recruit CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recruit-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage candidates, jobs, and client companies with Recruit CRM and AI agents.

## Description
### What you can do
- List and manage candidates in your recruitment database in real-time.
- Track job vacancies, requirements, and application pipelines.
- Access client company details and key contacts directly from your AI agent.
- Create new candidates and job postings with simple commands.

### How it works
1. Obtain your API Token from Recruit CRM under Admin Settings > Account Management > API Token.
2. Enter your API Token in Vinkius platform.
3. Start chatting with your Recruit CRM agent to automate your recruitment workflows.

### Who is it for?
- Recruitment agencies looking for automated ATS and CRM control.
- HR teams managing a high volume of candidates and job postings.
- Hiring managers tracking pipeline status and decision makers.


## Available Tools (11)
- **get_candidate_details**: Get details of a specific candidate
- **get_company_details**: Get details of a specific company
- **get_contact_details**: Get details of a specific contact
- **get_job_details**: Get details of a specific job
- **get_me**: Get account information
- **create_candidate**: Add a new candidate
- **create_job**: Create a new job posting
- **list_candidates**: List recruitment candidates
- **list_companies**: List client companies
- **list_contacts**: List client contacts
- **list_jobs**: List job vacancies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recruit CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs in Recruit CRM."

**🤖 AI Agent:**
> I've found 5 active jobs, including Software Engineer (ID: j1) and Product Manager (ID: j2).

---

**👤 You:**
> "Show me all candidates in the final interview stage across all open positions."

**🤖 AI Agent:**
> 14 candidates in final interview stage across 6 open positions. "Senior Backend Engineer": 3 candidates (top: Sarah Chen, 4.8/5 rating). "Product Manager": 2 candidates. "UX Designer": 3 candidates (final decision by Friday). "DevOps Lead": 2 candidates. "Sales Director": 2 candidates. "Data Analyst": 2 candidates. Average time in pipeline: 18 days. 5 candidates have competing offers with deadlines this week. 3 reference checks are pending completion.

---

**👤 You:**
> "Add a new candidate to the Senior Backend Engineer position and schedule a first-round interview."

**🤖 AI Agent:**
> Candidate added: Alex Rivera. Position: Senior Backend Engineer. Source: LinkedIn. Resume parsed: 8 years experience, Python/Go/AWS. Skills match: 92%. First-round interview scheduled: Thursday, May 22 at 10 AM with James Park (Engineering Manager). Calendar invite sent to candidate and interviewer. Interview scorecard template "Technical Assessment v3" attached. Candidate status: Active, Stage: Phone Screen.


## ❓ FAQ

**Q: How do I get my API Token?**
Log in to Recruit CRM and go to Admin Settings > Account Management > API Token to generate your token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recruit-crm](https://vinkius.com/mcp/recruit-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recruit CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recruit-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recruit CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recruit-crm": {
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
