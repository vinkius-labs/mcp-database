# DevSkiller MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devskiller)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage technical assessments, track candidates, and monitor test results via the DevSkiller API.

## Description
Integrate **DevSkiller**, the technical screening and talent assessment platform, directly into your AI workflow. Manage your candidate pipeline, send test invitations, and retrieve detailed assessment reports and skill scores using natural language.

### What you can do

- **Candidate Oversight** — List and search for candidates in your database and monitor their current assessment status.
- **Test Management** — Access your library of available technical tests, coding tasks, and quizzes.
- **Invitation Tracking** — Monitor sent test invitations and track candidate progress in real-time.
- **Performance Analytics** — Retrieve full assessment reports with granular skill scores and performance metrics.

### How it works

1. Connect the DevSkiller integration to your AI assistant.
2. Authorize using your DevSkiller API Key (found in your account settings).
3. Orchestrate your technical hiring and talent assessment through intuitive conversation.

### Who is this for?

- **Tech Recruiters** — Quickly check candidate scores and invitation statuses on the go.
- **Hiring Managers** — Review technical assessment reports and skill breakdowns via chat.
- **Talent Acquisition Teams** — Manage the candidate pipeline and send test invitations during planning.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and limits for your DevSkiller account
- **get_candidate_profile**: Get detailed information for a specific candidate
- **get_candidate_assessment_report**: Retrieve the full assessment report for a candidate
- **invite_candidate_to_test**: Send a new test invitation to a candidate
- **list_assessment_candidates**: List all candidates in your DevSkiller account
- **list_test_invitations**: List all sent test invitations and their current status
- **list_recently_sent_invitations**: List test invitations sent in the last 24 hours
- **list_available_tests**: List all assessment tests configured in your catalog
- **list_high_score_candidates**: Identify candidates who achieved a score above a specific threshold
- **search_candidates_by_identity**: Search for a candidate by name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DevSkiller** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all candidates who scored above 85% in recent tests."

**🤖 AI Agent:**
> I've found 3 candidates with scores above 85%: 'Alice Johnson' (92%), 'Bob Miller' (88%), and 'Kenji Tanaka' (86%). Would you like to see the detailed report for Alice?

---

**👤 You:**
> "Show me the assessment status for candidate 'john.doe@example.com'."

**🤖 AI Agent:**
> John Doe has currently completed 2 out of 3 tasks in the 'Senior Backend Developer' test. He has 15 minutes remaining. Should I notify you when he submits the final result?

---

**👤 You:**
> "Invite 'Sarah Smith' (sarah@example.com) to the 'Frontend React' test."

**🤖 AI Agent:**
> I've successfully sent an invitation to Sarah Smith for the 'Frontend React' test (ID: FR-101). She will receive an email with instructions shortly. Would you like me to track her progress?


## ❓ FAQ

**Q: How do I get a DevSkiller API Key?**
Log in to your DevSkiller account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from that section.

**Q: Can the agent show the candidate's code?**
This integration currently focuses on retrieving scores, statuses, and technical reports. Full source code review should be performed within the DevSkiller platform.

**Q: How do I invite a candidate via chat?**
You can use the invite_candidate_to_test tool. You will need to provide the candidate's email address and the specific Test ID from your catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devskiller](https://vinkius.com/mcp/devskiller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DevSkiller** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `devskiller` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DevSkiller** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devskiller": {
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
