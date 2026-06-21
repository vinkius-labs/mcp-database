# LearnWorlds MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/learnworlds)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Build and sell online courses with a white-label LMS that includes interactive video, community forums, and built-in marketing tools.

## Description
Connect your **LearnWorlds** account to any AI agent and take full control of your online academy orchestration and student productivity through natural conversation. LearnWorlds provides a powerful platform for creating and selling online courses, and this integration allows you to retrieve course metadata, manage student enrollments, and monitor academic progress directly from your chat interface.

### What you can do

- **Course & Content Orchestration** — List all managed courses and retrieve detailed module and unit metadata programmatically to ensure your learning roadmap is always synchronized.
- **User & Profile Intelligence** — Access and monitor student profiles and create new user accounts directly from the AI interface to maintain high-fidelity academic records.
- **Enrollment & Access Control** — Manually enroll students into specific courses or products via natural language to drive better promotional efficiency and class coordination.
- **Payment & Subscription Oversight** — List and oversee recent payments and retrieve detailed transaction metadata using simple AI commands to track your academy's revenue health.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your LMS workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your LearnWorlds Client ID, Client Secret, and School Domain from your admin panel
3. Start managing your academy from Claude, Cursor, or any MCP-compatible client

No more manual logging into the school dashboard for quick student or course checks. Your AI acts as a dedicated registrar or academic coordinator.

### Who is this for?

- **Course Creators & Academy Owners** — quickly retrieve enrollment summaries and monitor sales performance without switching apps.
- **Academic Coordinators** — automate the retrieval of student metadata and track course completion via natural conversation.
- **Developers** — integrate real-time LMS data and student intelligence directly within the chat.


## Available Tools
- **create_student**: Create a new student
- **enroll_student**: Enroll a student in a product
- **get_course_contents**: Get course contents
- **get_student_details**: Get student details
- **list_courses**: List all courses
- **list_payments**: List all payments
- **list_subscriptions**: List all student subscriptions
- **list_students**: List all students


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LearnWorlds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all courses with enrollment counts and the latest student activity."

**🤖 AI Agent:**
> Courses: 6. 'Web Development Bootcamp' (890 students, $199, 4.7★ ⭐). 'UX Design Course' (456, $149, 4.8★). 'Data Science Intro' (678, $99, 4.5★). 'Marketing Fundamentals' (234, $79, 4.3★). 'Python Mastery' (345, $129, 4.6★). 'Business Analytics' (123, $169, 4.4★). Total: 2,726 students. Latest: Sarah completed 'Web Dev' lesson 45 (3 min ago).

---

**👤 You:**
> "Show student progress and completion rates for the UX Design Course."

**🤖 AI Agent:**
> UX Design Course: 456 students. Completed: 198 (43%). In Progress: 189 (41%). Not Started: 69 (15%). Average progress: 58%. Completion rate trend: Jan (38%), Feb (40%), Mar (42%), Apr (43% ⬆️). Top students: Ana Costa (100%, certified), Mike Torres (95%), Lisa Park (88%). Average completion time: 6.2 weeks. Drop-off: Module 4 'User Research' (12% abandon rate).

---

**👤 You:**
> "Show new enrollments this week and school analytics."

**🤖 AI Agent:**
> New enrollments (7 days): 42. Web Dev: 15, UX Design: 10, Data Science: 8, Python: 5, Others: 4. Revenue: $6,890. School analytics: Total students: 2,726. Active (30 days): 1,890 (69%). Avg session: 28 min. Certificates issued (month): 34. Course completion rate: 41%. MRR: $12,400.


## ❓ FAQ

**Q: Can I track student progress and enrollments?**
Yes. Browse all students with course enrollment data, completion percentages, last activity, and engagement metrics.

**Q: Does LearnWorlds use OAuth2?**
Yes. LearnWorlds requires **Client ID**, **Client Secret**, and your **School Domain** (e.g., `your-school.learnworlds.com`). OAuth2 tokens are exchanged at `https://{domain}/admin/api/oauth2/token`.

**Q: Can I manage course content and settings?**
Yes. List courses with curricula, manage course settings, and access enrollment and pricing configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/learnworlds](https://vinkius.com/mcp/learnworlds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LearnWorlds** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `learnworlds` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LearnWorlds** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "learnworlds": {
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
