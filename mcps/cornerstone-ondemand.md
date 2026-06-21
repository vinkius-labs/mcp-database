# Cornerstone OnDemand MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cornerstone-ondemand)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage training, performance, and employee transcripts via the Cornerstone LMS API.

## Description
Integrate **Cornerstone OnDemand**, the leading human capital management and learning platform, directly into your AI workflow. Monitor employee development, audit training transcripts, and manage your talent catalog using natural language.

### What you can do

- **Learning & Catalog** — List available courses and training objects in your corporate catalog.
- **Employee Transcripts** — Retrieve and audit the learning history and certifications for any employee.
- **Performance Tracking** — List active performance reviews and competency goals.
- **Recruiting Insights** — Monitor internal and external job postings across departments.

### How it works

1. Connect the Cornerstone integration to your AI assistant.
2. Authorize using your OAuth Client ID, Secret, and portal Subdomain.
3. Audit and manage your talent development lifecycle via chat.

### Who is this for?

- **HR Managers** — Quickly audit employee certifications and training compliance.
- **L&D Teams** — Manage course availability and track learning engagement.
- **Department Heads** — Review team performance goals and active job openings.


## Available Tools (10)
- **get_course_details**: Touches content metadata and availability rule boundaries.

Get details for a specific training course
- **get_user_details**: Touches organizational hierarchy, contact information, and account settings boundaries.

Get full profile for a specific employee
- **list_courses**: Resolves course metadata, duration, and delivery method.

List available training courses
- **list_departments**: Resolves department IDs, names, and parent-child relationships.

List organizational departments
- **list_job_postings**: Resolves job title, location, department, and posting date.

List internal and external job openings
- **list_catalog**: Resolves learning object IDs, titles, descriptions, and training types.

List all learning objects in the catalog
- **list_performance_reviews**: Resolves review cycle IDs, status, and associated employee/manager pairs.

List active or past performance reviews
- **list_skills_inventory**: Resolves skill names, descriptions, and categories.

List all skills defined in the system
- **list_user_transcripts**: Resolves course enrollment status, completion dates, and scores.

List learning history and courses for a user
- **list_users**: Resolves properties such as user ID, name, email, department, and employment status.

List users in the Cornerstone portal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cornerstone OnDemand** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active training courses available in our learning catalog."

**🤖 AI Agent:**
> I've retrieved your corporate catalog. You have 120 active courses, including 'Cybersecurity Basics', 'Leadership 101', and 'Advanced Excel'. Would you like to filter them by category?

---

**👤 You:**
> "Show me the learning transcript for employee 'Jane Doe'."

**🤖 AI Agent:**
> I found Jane Doe's transcript. She has completed 15 courses and has 2 certifications active. Her most recent completion was 'Diversity & Inclusion' on March 15th. Should I list her pending requirements?

---

**👤 You:**
> "List all open job postings in the Engineering department."

**🤖 AI Agent:**
> There are 4 open positions in Engineering: 'Senior Backend Engineer', 'DevOps Lead', and two 'Frontend Developer' roles. Would you like to see the full descriptions for any of these?


## ❓ FAQ

**Q: How do I get Cornerstone OAuth credentials?**
You need to register an application in the Cornerstone Edge API portal or request Client ID and Secret from your system administrator.

**Q: What is the subdomain?**
It is the first part of your portal URL. For example, if you log in at 'company.csod.com', your subdomain is 'company'.

**Q: Can the agent assign courses to employees?**
This integration currently focuses on auditing and listing learning objects. Automated assignment would require additional write permissions and workflow configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cornerstone-ondemand](https://vinkius.com/mcp/cornerstone-ondemand)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cornerstone OnDemand** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cornerstone-ondemand` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cornerstone OnDemand** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cornerstone-ondemand": {
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
