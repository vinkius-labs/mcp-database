# Thinkific MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkific)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create and sell online courses with a platform that handles course hosting, student enrollment, and payment processing beautifully.

## Description
Connect your **Thinkific** LMS account to any AI agent and simplify how you manage your student directory, course catalog, and enrollment workflows through natural conversation.

### What you can do

- **Student Management** — List all registered users, create new student profiles, and retrieve detailed metadata for individual accounts.
- **Course Oversight** — List all courses, bundles, and products, and fetch detailed configurations for specific learning materials.
- **Enrollment Automation** — Programmatically enroll students in specific courses or bundles with optional expiry dates via AI.
- **Order Tracking** — Monitor your site's commercial performance by listing orders and transaction history.
- **Content Organization** — Query course categories and products to understand your learning ecosystem's structure.
- **Operational Maintenance** — Verify student data and course availability directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Thinkific API Key and Subdomain (found in your account settings)
3. Start managing your online academy from Claude, Cursor, or any MCP client

### Who is this for?

- **Course Creators & Educators** — quickly retrieve student lists and check course metadata via simple AI commands.
- **Customer Support Teams** — enroll students manually and verify order history directly from the workspace.
- **Academy Administrators** — monitor enrollment growth and manage user profiles via the AI assistant.


## Available Tools (10)
- **get_user**: Get details for a specific user
- **list_categories**: List course categories
- **list_courses**: List all courses
- **list_enrollments**: List user enrollments
- **list_orders**: List site orders
- **list_products**: List all products (Courses and Bundles)
- **list_users**: List Thinkific users
- **enroll_user**: Enroll a user in a product
- **create_user**: Requires email, first name, and last name.

Create a new user
- **get_course**: Get details for a specific course


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thinkific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active courses in my Thinkific academy."

**🤖 AI Agent:**
> I've retrieved your courses. You have 5 active learning materials including 'AI Fundamentals', 'Advanced React', and 'Business Strategy'. Which one would you like to see enrollments for?

---

**👤 You:**
> "Show me the details for student 'John Doe' (ID: user_10293)."

**🤖 AI Agent:**
> I've fetched John Doe's profile. He has been a member since Jan 2024 and is currently enrolled in 2 courses: 'AI Fundamentals' (90% complete) and 'Digital Marketing'. Shall I enroll him in another course?

---

**👤 You:**
> "Enroll user 'user_8823' into course 'course_5521' and set it to expire in 30 days."

**🤖 AI Agent:**
> Enrollment successful! I've added user_8823 to course_5521. The enrollment is set to expire on 2024-12-01. The student will receive a notification in their dashboard.


## ❓ FAQ

**Q: Can I manually enroll a student in a course using the AI?**
Yes! Use the `enroll_user` tool. Provide the User ID and the Course ID to instantly create a new enrollment for that student in your Thinkific academy.

**Q: How do I see the full list of registered students?**
Run the `list_users` query. You can optionally use the `page` and `limit` parameters to navigate through your entire student directory.

**Q: Is it possible to check recent revenue or orders via AI?**
Absolutely. Use the `list_orders` query. Your agent will retrieve the history of all transactions and orders processed through your Thinkific site.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkific](https://vinkius.com/mcp/thinkific)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thinkific** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thinkific` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thinkific** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thinkific": {
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
