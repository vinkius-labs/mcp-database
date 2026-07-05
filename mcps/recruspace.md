# RecruSpace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recruspace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate recruitment via RecruSpace — manage candidates, track talent pools, and monitor job posts directly.

## Description
Connect your **RecruSpace** account to any AI agent to streamline your hiring and talent orchestration through natural conversation. RecruSpace provides a modern recruitment platform for programmatically managing candidates, organizing talent pools, and tracking job post statuses through its robust API.

### What you can do

- **Candidate & Applicant Orchestration** — List all managed candidates and add new potential hires with detailed profile metadata programmatically.
- **Talent Pool Intelligence** — Access and monitor your talent pools and create new collections to organize your recruitment pipeline directly from the AI interface.
- **Job Post Lifecycle Management** — List all active job posts and retrieve detailed metadata to maintain a clear overview of your hiring needs via natural language.
- **Candidate Deep-Dive** — Retrieve granular details for specific candidates to understand full context and qualification metrics.
- **Operational Monitoring** — Track system activity and manage recruitment metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your RecruSpace API Key from your account settings
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

No more manual status checking or spreadsheet candidate tracking. Your AI acts as a dedicated recruitment coordinator or HR lead.

### Who is this for?

- **HR Managers & Recruiters** — quickly retrieve candidate summaries and monitor talent pool growth without switching apps.
- **Hiring Operations Teams** — automate the ingestion of new candidates and track qualification stages via natural conversation.
- **Developers** — integrate real-time recruitment data and talent intelligence into custom business dashboards.


## Available Tools (11)
- **add_candidate**: Pass data as a JSON string.

Add a new candidate
- **create_talent_pool**: Create a new talent pool
- **get_job**: Get details for a specific job posting
- **get_talent_pool**: Get details for a talent pool
- **list_candidates**: List all candidates
- **list_interviews**: List all scheduled interviews
- **list_jobs**: List all job posts
- **list_pipelines**: List all hiring pipelines
- **list_talent_pools**: List all talent pools
- **update_candidate**: Update candidate information
- **get_candidate_details**: Get specific candidate details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RecruSpace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active candidates in RecruSpace."

**🤖 AI Agent:**
> I've retrieved your candidates. You have 15 active applicants including 'Alice Miller' and 'Robert Chen'. Would you like to see the qualification score for any of them?

---

**👤 You:**
> "Show me all active job postings with their application counts and pipeline status."

**🤖 AI Agent:**
> 9 active job postings. "Full Stack Developer" leads with 87 applications (12 in screening, 5 interviewing, 2 in final round). "Marketing Manager" has 45 applications (8 screening). "Data Engineer" received 34 applications in 5 days. "Customer Success": 28 applications. 5 additional positions with combined 112 applications. Total active candidates: 306. Average time to first response: 2.3 days. 4 positions have been open for 30+ days and may need refreshed descriptions.

---

**👤 You:**
> "Add a new candidate to the talent pool for future engineering roles."

**🤖 AI Agent:**
> Candidate added to "Future Engineering Talent" pool. Name: Lisa Wang. Skills: React, TypeScript, Node.js, AWS. Experience: 5 years. Source: Tech Conference referral. The talent pool now has 134 candidates. Lisa has been tagged with "Frontend", "Cloud", and "Mid-Senior". An automated nurture email sequence will begin in 24 hours with company culture content. You'll be notified when matching positions open.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific candidate by providing their ID?**
Yes! Use the `get_candidate_details` tool with the Candidate ID. Your agent will respond with the complete metadata for the profile, including qualifications and status in seconds.

**Q: How do I find my RecruSpace API Key?**
Log in to your RecruSpace account, navigate to the **Settings** or **API** section, and you will find your unique secret API key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recruspace](https://vinkius.com/mcp/recruspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RecruSpace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recruspace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RecruSpace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recruspace": {
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
