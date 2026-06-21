# HRBlade MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hrblade)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Streamline recruitment with an ATS that manages job postings, candidate pipelines, and interview scheduling for growing teams.

## Description
Connect your **HRBlade** account to any AI agent and manage asynchronous video interviews through natural conversation.

### What you can do

- **Interview Templates** — List all interview templates and create new ones with custom questions, time limits, and instructions
- **Candidate Invitations** — Send video interview invitations to candidates by email with personalized details
- **Candidate Management** — Browse all candidates in your pipeline and inspect individual profiles with status
- **Response Review** — List all submitted video responses to review candidate answers and evaluate performance

### How it works

1. Subscribe to this server
2. Enter your HRBlade API Key from your account settings
3. Start managing interviews from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — create interview templates, send invitations, and review video responses without switching to the dashboard
- **Hiring Managers** — evaluate candidate responses and track pipeline progress through AI
- **HR Teams** — scale asynchronous interviewing and manage high-volume candidate screening


## Available Tools
- **create_interview**: Pass data as a JSON string.

Create a new interview template
- **get_candidate_details**: Get specific candidate details
- **list_candidates**: List all recruiting candidates
- **list_interviews**: List all interview templates
- **list_interview_responses**: List all candidate video responses
- **send_interview_invitation**: Pass data as a JSON string.

Send an invitation to a candidate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HRBlade** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 'Senior Developer' interview with 3 technical questions and send it to 2 candidates."

**🤖 AI Agent:**
> Interview template created! Title: 'Senior Developer — Technical Screen', ID: int_4521. Questions: 1) 'Describe your approach to designing scalable microservices architectures.' (3 min limit). 2) 'Walk us through how you would debug a production performance issue.' (3 min). 3) 'Explain a complex technical decision you made recently and the trade-offs involved.' (3 min). Invitations sent: 1) sarah.chen@email.com (Sarah Chen) — ✅ Invitation delivered. 2) mike.torres@email.com (Mike Torres) — ✅ Invitation delivered. Both candidates will receive a link to record their video responses at their convenience. You now have 8 active interview templates. Would you like to review pending responses?

---

**👤 You:**
> "Show all candidates in my pipeline and the latest video responses."

**🤖 AI Agent:**
> Your pipeline: 24 candidates total. By status: Invited (8), Responded (12), Reviewed (3), Hired (1). Latest video responses: 1) Ana Costa — 'Product Manager' interview, submitted 2 hours ago. 3 answers recorded (avg 2:15 each). 2) James Rodriguez — 'Senior Developer' interview, submitted yesterday. 3 answers (avg 2:45). 3) Lisa Park — 'UX Designer' interview, submitted 2 days ago. 4 answers (avg 1:50). Pending invitations: 5 candidates haven't opened their invitation yet. Would you like to get details for a specific candidate or send reminders?

---

**👤 You:**
> "List all interview templates and show which ones have pending responses to review."

**🤖 AI Agent:**
> Interview templates: 8 total. Active: 1) 'Senior Developer — Technical Screen' (int_4521, 3 questions, 12 invited, 8 responded, 4 pending review). 2) 'Product Manager — Case Study' (int_4518, 4 questions, 8 invited, 6 responded, 3 pending). 3) 'UX Designer — Portfolio Review' (int_4515, 5 questions, 6 invited, 5 responded, 2 pending). 4) 'Sales Rep — Pitch Exercise' (int_4510, 3 questions, 15 invited, 10 responded, 5 pending). Archived: 4 templates. Total pending reviews: 14 video responses. Would you like to start reviewing or create a new template?


## ❓ FAQ

**Q: Can I create an interview template and send invitations to candidates?**
Yes. Use `create_interview` with a JSON payload containing the title, description, and an array of questions. Then use `send_interview_invitation` with the candidate's email, first name, last name, and the interview ID. The candidate will receive an email with a link to record their video responses.

**Q: Can I review all video responses submitted by candidates?**
Yes. The `list_interview_responses` tool retrieves all submitted video responses with candidate details, interview template reference, and submission timestamps. Use `get_candidate_details` to inspect a specific candidate's full profile and response history.

**Q: How does asynchronous video interviewing work with HRBlade?**
HRBlade enables one-way video interviews where candidates record responses at their own pace. You create a template with questions, send an invitation, and the candidate records video answers through a web link. You can then review all responses asynchronously without scheduling live calls. Use `list_interviews` to see all templates and `list_candidates` to track your pipeline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hrblade](https://vinkius.com/mcp/hrblade)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HRBlade** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hrblade` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HRBlade** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hrblade": {
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
