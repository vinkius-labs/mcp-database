# eduMe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edume)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage mobile training, track trainees, and monitor course completion via the eduMe API.

## Description
Integrate **eduMe**, the leading mobile-first training platform for the deskless workforce, directly into your AI workflow. Manage your training courses and modules, track trainee profiles and completion rates, monitor team performance, and oversee your organizational learning metadata using natural language.

### What you can do

- **Course Oversight** — List and retrieve detailed information and completion metrics for all your mobile training courses.
- **Trainee Intelligence** — Monitor user training profiles, identifying completed courses, active enrollments, and organizational team memberships.
- **Team Management** — Access and monitor all training teams and user groups configured in your eduMe account.
- **Learning Auditing** — Retrieve high-level summaries of team activity, course engagement, and organizational training health.

### How it works

1. Connect the eduMe integration to your AI assistant.
2. Authorize using your eduMe API Key (found in your account settings).
3. Orchestrate your mobile training operations and workforce development through intuitive conversation.

### Who is this for?

- **Training Managers** — Quickly check course completion rates and team activity on the go.
- **Operations Leads** — Monitor workforce readiness and training coverage via chat.
- **HR Administrators** — Research individual trainee history and team memberships instantly.


## Available Tools (10)
- **get_edume_account_metadata**: Retrieve metadata and limits for your eduMe account
- **get_course_details**: Get detailed settings and module list for a specific training course
- **quick_team_training_audit**: Retrieve a high-level summary of team activity and member counts
- **get_user_training_profile**: Get full training history and profile for a specific user
- **list_training_courses**: List all mobile training courses available in eduMe
- **list_top_performing_courses**: Identify courses with the highest completion or engagement rates (mock logic)
- **list_latest_training_content**: Identify the most recently created or updated training courses
- **list_training_teams**: List all teams and user groups configured in your eduMe account
- **list_trained_users**: List all users registered in your eduMe training platform
- **search_trainees_by_keyword**: Search for users using a name keyword or external identifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eduMe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mobile training courses."

**🤖 AI Agent:**
> I've found several courses, including 'Company Onboarding', 'Safety Essentials', and 'Customer Service Excellence'. 'Safety Essentials' has a 95% completion rate. Would you like to see the details for Onboarding?

---

**👤 You:**
> "Show me the training profile for user 'john_doe'."

**🤖 AI Agent:**
> John Doe has completed 4 out of 5 assigned courses. They are a member of the 'Sales - North' team and last logged in today. Should I list the specific courses they have finished?

---

**👤 You:**
> "Which teams have the lowest course engagement?"

**🤖 AI Agent:**
> The 'Warehouse Night Shift' and 'Regional Drivers' teams currently have the lowest engagement rates (below 60%). Would you like me to pull the contact information for the team leads?


## ❓ FAQ

**Q: How do I get an eduMe API Key?**
Log in to your eduMe dashboard, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. API access may require an enterprise-level plan.

**Q: Can the agent assign courses to users?**
This integration currently focuses on listing and auditing training data. Assigning courses or creating new users should be managed via the eduMe dashboard or specific enrollment API endpoints.

**Q: Does the integration show real-time completion?**
Yes, you can use the list_training_courses or get_user_training_profile tools to retrieve the latest completion rates and statuses as reported by the eduMe platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edume](https://vinkius.com/mcp/edume)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eduMe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `edume` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eduMe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edume": {
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
