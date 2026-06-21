# DigitalChalk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digitalchalk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to manage LMS offerings, track learner progress, and monitor exam results via the DigitalChalk API.

## Description
Integrate **DigitalChalk**, the comprehensive learning management system (LMS), directly into your AI workflow. Manage your course offerings, monitor student enrollments and completion statuses, and track exam results using natural language.

### What you can do

- **Offering Oversight** — List and retrieve detailed settings for all your active course offerings in the catalog.
- **Learner Intelligence** — Access detailed profiles for students and administrators and track their learning history.
- **Progress Tracking** — Monitor individual enrollment progress and identify recently completed courses.
- **Assessment Monitoring** — List exams and quizzes and track results to ensure academic compliance.

### How it works

1. Connect the DigitalChalk integration to your AI assistant.
2. Authorize using your DigitalChalk API Key and portal Subdomain.
3. Orchestrate your online learning and talent development through intuitive conversation.

### Who is this for?

- **L&D Managers** — Quickly check enrollment numbers and learner progress on the go.
- **Training Administrators** — Research user profiles and course offerings via chat.
- **Hiring & Onboarding Teams** — Monitor progress of new hire certification plans instantly.


## Available Tools
- **get_lms_account_metadata**: Retrieve metadata and settings for your DigitalChalk account
- **list_high_performing_learners**: Identify enrollments with a grade above a certain percentage (mock logic)
- **get_offering_details**: Get detailed settings and information for a specific course offering
- **get_user_learning_profile**: Get full profile and enrollment history for a specific user
- **list_user_enrollments**: List all courses a specific user is currently enrolled in
- **list_assessment_exams**: List all exams and quizzes defined in the system
- **list_course_offerings**: List all available course offerings in your DigitalChalk catalog
- **list_recent_course_completions**: Identify enrollments that have been recently completed (mock logic)
- **list_lms_users**: List all students and administrators registered in your DigitalChalk account
- **search_users_by_identity**: Search for a user by their full name or email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DigitalChalk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active course offerings."

**🤖 AI Agent:**
> I've found 15 active offerings, including 'Python for Beginners', 'Project Management 101', and 'Business Ethics'. Would you like to see the pricing for any of these?

---

**👤 You:**
> "Show me the grade for user 'John Doe' in 'Business Ethics'."

**🤖 AI Agent:**
> John Doe achieved a grade of 92% in 'Business Ethics'. He completed the course on June 12th. Should I check if his certificate has been issued?

---

**👤 You:**
> "Search for users with email '@example.com'."

**🤖 AI Agent:**
> I've found 3 users matching '@example.com': 'Alice Smith', 'Bob Miller', and 'Charlie Brown'. Which profile would you like me to pull up for you?


## ❓ FAQ

**Q: How do I get a DigitalChalk API Key?**
Log in to your DigitalChalk account, navigate to the API section in your settings, and you can generate or retrieve your unique API Key from there.

**Q: What is the subdomain?**
It is the first part of your DigitalChalk URL. For example, if you access your portal at 'mycompany.digitalchalk.com', your subdomain is 'mycompany'.

**Q: Can the agent see exam answers?**
The agent can retrieve overall exam results and grades, but specific question-level answers and individual choices are viewed within the DigitalChalk platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digitalchalk](https://vinkius.com/mcp/digitalchalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DigitalChalk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `digitalchalk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DigitalChalk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digitalchalk": {
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
