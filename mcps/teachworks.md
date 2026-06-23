# Teachworks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teachworks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calendar-scheduling](../categories/calendar-scheduling.md)

Schedule tutoring sessions, manage student progress, and handle billing for tutoring businesses and learning centers.

## Description
Connect your **Teachworks** tutoring management account to any AI agent and simplify how you coordinate your education business, student directory, and lesson scheduling through natural conversation.

### What you can do

- **Student Management** — List all enrolled students, create new student profiles, and retrieve detailed academic metadata.
- **Teacher Coordination** — Query your directory of tutors and teachers to manage staff assignments and availability.
- **Lesson Scheduling** — List all scheduled lessons and classes to monitor your academy's teaching calendar.
- **Family Oversight** — List and manage customer families to maintain organized billing and contact records.
- **Profile Insights** — Fetch detailed profile information for individual students using their unique IDs.
- **Operational Monitoring** — Check your education ecosystem status and teacher distributions directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Teachworks API Token (found in your account settings)
3. Start managing your tutoring business from Claude, Cursor, or any MCP client

### Who is this for?

- **Tutoring Business Owners** — quickly retrieve student lists and monitor teaching schedules via simple AI commands.
- **Academy Administrators** — coordinate teacher availability and manage family records directly from the workspace.
- **Education Coordinators** — verify student details and verify lesson assignments via the AI assistant.


## Available Tools (6)
- **create_student**: Add a new student
- **get_student**: Get student details
- **list_families**: List families
- **list_lessons**: List scheduled lessons
- **list_students**: List all students in Teachworks
- **list_teachers**: List all teachers (tutors)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teachworks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active students in my Teachworks account."

**🤖 AI Agent:**
> I've retrieved your student list. You have 25 active students including 'John Doe', 'Jane Smith', and 'Alex Rivera'. Which one would you like more details on?

---

**👤 You:**
> "Show me the teaching schedule for this week."

**🤖 AI Agent:**
> I've fetched the lesson list. This week you have 12 scheduled lessons, including 'Math Level 1' (Tue, 3 PM) and 'Intro to AI' (Wed, 10 AM). Shall I retrieve the details for any specific class?

---

**👤 You:**
> "Create a new student record for 'Mike Ross' (mike@example.com)."

**🤖 AI Agent:**
> Success! The student record for Mike Ross (mike@example.com) has been created in Teachworks with ID user_10293. I've added him to your directory.


## ❓ FAQ

**Q: Can I see all the lessons scheduled for my academy via AI?**
Yes! Use the `list_lessons` tool. Your agent will retrieve the complete enseñante calendar, including scheduled times and associated students.

**Q: How do I add a new student to my directory?**
Use the `create_student` action. Provide the first name, last name, and an optional email to register the new student record in Teachworks instantly.

**Q: Is it possible to see which families are registered via AI?**
Absolutely. Use the `list_families` query. The agent will retrieve the directory of customer families associated with your business.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teachworks](https://vinkius.com/mcp/teachworks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teachworks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teachworks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teachworks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teachworks": {
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
