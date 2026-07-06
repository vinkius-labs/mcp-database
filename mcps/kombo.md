# Kombo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kombo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Unified API for HRIS, ATS, and LMS — manage employees, job openings, and training courses across 50+ platforms through a single interface.

## Description
Connect your entire HR and recruitment stack to any AI agent using **Kombo**. This server provides a unified interface to interact with HRIS, ATS, and LMS systems, allowing you to manage the entire employee lifecycle through natural conversation.

### What you can do

- **HRIS Management** — Retrieve employee records, track absences (vacation/sick leave), and list organizational groups or locations.
- **Recruitment (ATS)** — Query job openings, manage candidate profiles, and track applications or interview stages across different providers.
- **Learning & Training (LMS)** — List available courses, manage user enrollments, and sync training data in bulk.
- **Assessments** — Handle assessment packages and update order results directly from your agent.
- **Unified Access** — Use a single API key to interact with multiple integrations without worrying about individual provider schemas.

### How it works

1. Subscribe to this server
2. Enter your Kombo API Key
3. (Optional) Provide a specific Integration ID to target a connection
4. Start managing your workforce data from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Operations** — quickly pull employee lists or absence reports without logging into multiple HR portals.
- **Recruiters** — check job statuses and candidate details directly from your workflow tools.
- **L&D Managers** — monitor course catalogs and user progress across learning platforms.


## Available Tools (21)
- **get_ats_applications**: Retrieve job applications from the ATS
- **get_ats_candidates**: Retrieve candidate profiles from the ATS
- **create_ats_application**: Create a new application and candidate for a job
- **get_ats_interviews**: List scheduled interviews from the ATS
- **get_ats_jobs**: Retrieve all job openings from the ATS
- **get_ats_rejection_reasons**: List reasons for rejecting applications in the ATS
- **get_ats_roles**: List system and job roles in the ATS
- **get_ats_users**: List ATS users (recruiters, hiring managers)
- **get_hris_absence_types**: List available absence types in the HRIS
- **get_hris_absences**: Retrieve employee absences (vacation, sick leave, etc.)
- **create_hris_employee_form**: Create an employee using a tool-specific form
- **get_hris_employees**: Supports pagination and filtering.

Retrieve all employees from the HRIS
- **get_hris_groups**: Retrieve organizational groups (teams, departments)
- **get_hris_legal_entities**: List legal entities in the HRIS
- **get_hris_locations**: List work locations in the HRIS
- **get_lms_courses**: Retrieve available courses from the LMS
- **upsert_lms_courses_bulk**: Asynchronously upsert courses into the LMS
- **get_lms_users**: Retrieve learners from the LMS
- **passthrough_request**: Call the native API of the underlying tool directly
- **put_assessment_order_result**: Write back results for an assessment order
- **put_assessment_packages**: Define available assessment/background check packages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kombo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the HRIS updated since last month."

**🤖 AI Agent:**
> I've retrieved the employee list. There are 12 records updated since last month, including 'Jane Doe' and 'John Smith'. Would you like to see the full details for any of them?

---

**👤 You:**
> "Show me all active job openings from the ATS."

**🤖 AI Agent:**
> I found 5 active job openings: Senior Backend Engineer, Product Manager, UX Designer, and 2 others. Which one should I provide more info on?

---

**👤 You:**
> "Get all available absence types from the HR system."

**🤖 AI Agent:**
> The system lists the following absence types: Vacation, Sick Leave, Parental Leave, and Unpaid Leave. Do you need to check the absences for a specific employee?


## ❓ FAQ

**Q: Can I list all employees from my HRIS system using this server?**
Yes! Use the `get_hris_employees` tool. You can also apply filters like `updated_after` to find recently modified records or use pagination for large datasets.

**Q: How do I check for active job openings in our connected ATS?**
Simply ask the agent to run the `get_ats_jobs` tool. It will retrieve all job openings, including metadata like descriptions and status, from your integrated recruitment platform.

**Q: Is it possible to see why a candidate was rejected?**
Yes, the `get_ats_rejection_reasons` tool allows you to list the configured rejection reasons in your ATS, helping you understand the hiring outcomes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kombo](https://vinkius.com/mcp/kombo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kombo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kombo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kombo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kombo": {
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
