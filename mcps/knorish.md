# Knorish MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knorish)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/knorish-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/knorish-mcp)
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


## Available Tools
- **create_user**: Create a new user
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


## Installation & Usage

To install and use the **Knorish** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knorish](https://vinkius.com/mcp/knorish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
