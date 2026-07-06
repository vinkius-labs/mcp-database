# Knorish MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knorish)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Launch your online school and sell courses with a platform that bundles LMS, website builder, and payment processing together.

## Description
Connect your **Knorish** account to any AI agent and manage your online course business through natural conversation.

### What you can do

- **Course Management** — List courses, inspect curricula, and track enrollment numbers
- **Student Tracking** — Browse students with progress, completion rates, and engagement
- **Enrollment Monitoring** — Track new enrollments, active students, and drop-offs
- **Content Browsing** — Navigate course modules, lessons, and media content
- **Sales Analytics** — Monitor revenue, orders, and conversion metrics
- **Certificate Management** — Track certificate issuance and completion records

### How it works

1. Subscribe to this server
2. Enter your Knorish App ID and App Key
3. Start managing courses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Course Creators** — manage courses and track student progress
- **Educators** — monitor enrollments and completion rates
- **EdTech Businesses** — analyze sales and optimize course offerings


## Available Tools (12)
- **create_webhook**: Create a new webhook
- **enroll_user**: Enroll a user in a course
- **get_account_info**: Get academy account details
- **get_course**: Get course details
- **get_student_progress**: Get student progress
- **get_user**: Get user details
- **list_bundles**: List course bundles
- **list_courses**: List all courses
- **list_users**: List all users
- **list_webhooks**: List webhooks
- **unenroll_user**: Unenroll a user from a course
- **create_user**: Create a new user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knorish** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all courses with enrollment numbers and the top-performing course."

**🤖 AI Agent:**
> Courses: 6. 'Digital Marketing Masterclass' (1.2K students, $89, 4.8★ ⭐ top). 'Python for Beginners' (890, $49, 4.6★). 'Business Strategy' (456, $149, 4.7★). 'UX Design Fundamentals' (678, $79, 4.5★). 'Data Analytics' (234, $129, 4.4★). 'Leadership Skills' (123, $69, 4.3★). Total: 3,581 students. Revenue: $287K.

---

**👤 You:**
> "Show student progress for the Digital Marketing course and recent enrollments."

**🤖 AI Agent:**
> Digital Marketing: 1,200 students. Completion: 42% average. Completed: 504 (42%). In Progress: 480 (40%). Not Started: 216 (18%). Top students: Sarah Chen (100%, certificate issued), Mike Torres (95%), Lisa Park (88%). Recent enrollments (7 days): 28. Daily avg: 4. Drop-off rate: 12%.

---

**👤 You:**
> "Show the curriculum of the Python course and sales for this month."

**🤖 AI Agent:**
> Python for Beginners: 8 modules. 1) 'Introduction' (3 lessons, 45 min). 2) 'Variables & Types' (4 lessons, 60 min). 3) 'Control Flow' (5 lessons, 75 min). 4) 'Functions' (4 lessons, 60 min). 5) 'Data Structures' (6 lessons, 90 min). 6) 'OOP' (5 lessons, 80 min). 7) 'Projects' (3 lessons, 120 min). 8) 'Final Exam'. Total: 30 lessons, 8.5 hours. This month's sales: 42 orders, $2,058. Refunds: 2 ($98).


## ❓ FAQ

**Q: Can I track student progress and completion rates?**
Yes. Browse all students with course progress percentages, lesson completion, time spent, and engagement metrics. Track completion certificates.

**Q: Does Knorish require two credentials?**
Yes. Knorish requires an **App ID** and **App Key** pair for authentication against `api.knorish.com/v1`.

**Q: Can I monitor sales and enrollment analytics?**
Yes. Track total revenue, order counts, conversion rates, enrollment trends, and refund rates across all courses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knorish](https://vinkius.com/mcp/knorish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knorish** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knorish` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knorish** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knorish": {
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
