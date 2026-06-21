# Classe365 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/classe365)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/classe365-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/classe365-mcp)
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


## Installation & Usage

To install and use the **Classe365** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/classe365](https://vinkius.com/mcp/classe365)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
