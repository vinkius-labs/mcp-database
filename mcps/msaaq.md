# MSAAQ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/msaaq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage courses, enrollments, and student progress via MSAAQ directly from your AI agent.

## Description
Empower your AI agent with access to the **MSAAQ** Learning Management System (LMS) to automate your educational workflows and student management.

### What you can do

- **Course Management (Admin)** — List all courses and retrieve detailed engagement and enrollment statistics.
- **Student Oversight** — Manage user accounts, create new student profiles, and manually enroll students into courses.
- **Learning Experience** — Access available learning courses, module metadata, and monitor student progress.
- **Certification Tracking** — List earned certificates and verify the authenticity of issued course completions via UUID.

### How it works

1. Subscribe to this server
2. Enter your MSAAQ Access Token from your dashboard
3. Start managing your LMS platform from Claude, Cursor, or any MCP client

### Who is this for?

- **Education Administrators** — Quickly enroll students and check course stats via natural language.
- **Content Creators** — Monitor student engagement and manage course metadata efficiently.
- **Learners & Students** — Check personal enrollments and access earned certificates without leaving your workspace.


## Available Tools (12)
- **get_learning_course_details**: Get details for a course
- **list_all_courses_admin**: List all courses (Admin)
- **list_registered_users_admin**: List all students and users
- **list_student_certificates**: List my earned certificates
- **list_available_learning_courses**: List courses for students
- **verify_issued_certificate**: Verify a certificate authenticity
- **check_api_connectivity**: Verify MSAAQ API status
- **create_new_student_account**: Requires name and email.

Invite or create a new user
- **enroll_student_in_course**: Enroll a user into a course
- **get_course_performance_stats**: Get analytics for a course
- **get_my_active_enrollments**: List my enrolled courses
- **get_logged_in_user_profile**: Get current user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MSAAQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active courses in my MSAAQ admin panel."

**🤖 AI Agent:**
> I've found 5 active courses. Notable ones include 'Intro to AI' (ID: crs_123) and 'Advanced RAG' (ID: crs_456). Would you like stats on any of these?

---

**👤 You:**
> "Enroll student 'John Doe' (ID: usr_789) into the 'Advanced RAG' course."

**🤖 AI Agent:**
> Done! I've successfully enrolled John Doe into the Advanced RAG course (crs_456).

---

**👤 You:**
> "Show me my course completion certificates."

**🤖 AI Agent:**
> I've retrieved 2 certificates. You've completed 'Basic Python' and 'Data Science 101'. You can download or verify them here.


## ❓ FAQ

**Q: How do I get an Access Token for MSAAQ?**
Log in to your MSAAQ dashboard and navigate to the API or Developer portal section to generate your unique OAuth2 access token.

**Q: Can the agent enroll students into courses?**
Yes, using the `enroll_student_in_course` tool, the agent can manually register students into specific courses.

**Q: Is it possible to verify certificates?**
Absolutely. The `verify_issued_certificate` tool allows the agent to check the validity of any certificate issued by the platform using its UUID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/msaaq](https://vinkius.com/mcp/msaaq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MSAAQ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `msaaq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MSAAQ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "msaaq": {
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
