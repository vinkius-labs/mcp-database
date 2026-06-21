# Classe365 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/classe365)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Run your educational institution with student information management, admissions tracking, and academic planning in one platform.

## Description
Connect your **Classe365** student management system to any AI agent and simplify how you coordinate your educational institution, student directory, and academic records through natural conversation.

### What you can do

- **Student Lifecycle** — List all students, create new academic profiles, and retrieve detailed metadata for individual enrollments.
- **Academic Oversight** — List academic departments, sections, and classes to understand your institution's hierarchy.
- **Performance Monitoring** — List and query student attendance history and exam assessment scores via AI.
- **School Operations** — Verify configured subjects and class distributions directly from the agent.
- **Data Insights** — Fetch complete student metadata including contact info and course progress.
- **Administrative Efficiency** — Automate student registrations and record-keeping without leaving your workspace.

### How it works

1. Subscribe to this server
2. Enter your Classe365 Subdomain and API Key (found in your school settings)
3. Start managing your academy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **School Administrators** — quickly check student enrollment data and monitor attendance via simple AI commands.
- **Academic Coordinators** — verify class distributions and retrieve student performance reports directly from the workspace.
- **Registrar Teams** — automate student record creation and verify academic metadata via the AI assistant.


## Available Tools
- **create_student_profile**: Add a new student
- **get_student_details**: Get details for a specific student
- **list_academic_records**: List academic departments and sections
- **list_exam_assessments**: List assessments and scores
- **list_student_attendance**: List student attendance history
- **list_school_classes**: List configured classes
- **list_students**: List Classe365 students


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Classe365** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active students in my school account."

**🤖 AI Agent:**
> I've retrieved the student directory. You have 45 active enrollments including 'John Doe', 'Sarah Miller', and 'Mike Ross'. Which one would you like to see the academic profile for?

---

**👤 You:**
> "Show me the attendance record for student 'std_10293'."

**🤖 AI Agent:**
> Fetching attendance... Student std_10293 has a 95% attendance rate this semester with only 2 absences recorded in 'Mathematics'. Would you like the full log of dates?

---

**👤 You:**
> "Create a student profile for 'Anna White' (anna@example.com)."

**🤖 AI Agent:**
> Success! The profile for Anna White (anna@example.com) has been created in Classe365 with ID std_88231. She is now registered in your student directory.


## ❓ FAQ

**Q: Can I check a student's attendance history via AI?**
Yes! Use the `list_student_attendance` tool and provide the Student ID. Your agent will retrieve the complete attendance record for that student.

**Q: How do I add a new student to the SIS using the agent?**
Use the `create_student_profile` action. Provide the first name, last name, and email to register the new student record in Classe365 instantly.

**Q: Is it possible to see exam scores via AI?**
Absolutely. Use the `list_exam_assessments` query. The agent will retrieve a list of assessments and scores recorded in your academy's account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/classe365](https://vinkius.com/mcp/classe365)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Classe365** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `classe365` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Classe365** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "classe365": {
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
