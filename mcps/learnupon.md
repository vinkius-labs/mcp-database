# LearnUpon MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/learnupon)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/learnupon-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/learnupon-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage users, courses, and enrollments via the LearnUpon LMS API.

## Description
Connect your **LearnUpon** portal to any AI agent to automate your learning management operations. This MCP server enables your agent to interact with learner accounts, course catalogs, and enrollment data directly.

### What you can do

- **Learner Management** — List and search for users, and automate the creation or updating of learner profiles
- **Course Discovery** — Query your entire course library and search for specific training content by name
- **Enrollment Automation** — Manage user enrollments, link learners to courses, and handle unenrolling when needed
- **Progress Tracking** — Monitor enrollment statuses and identify learner participation across your portal
- **Bulk Operations Support** — Retrieve paginated lists of data to maintain large-scale learning environments

### How it works

1. Subscribe to this server
2. Enter your LearnUpon Subdomain, API Key ID, and API Key Secret
3. Start managing your LMS from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **LMS Administrators** — Quickly provision users and manage enrollments via natural language commands
- **L&D Managers** — Monitor course availability and learner progress without logging into the portal
- **HR Specialists** — Automate the onboarding of new hires into specific training paths effortlessly


## Available Tools
- **list_courses**: List all available courses
- **enroll_user_in_course**: Requires course_id and user identification.

Enroll a user into a specific course
- **create_user**: Requires email/username, password, and name.

Create a new learner account
- **unenroll_user**: Remove a user enrollment from a course
- **list_enrollments**: List all course enrollments
- **search_courses**: Search for courses by name
- **search_users**: Search for users by email or username
- **update_user**: Update an existing user account
- **list_users**: Use this to identify user IDs for enrollment or updates.

List all learner accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LearnUpon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the user with email 'learner@example.com' in LearnUpon."

**🤖 AI Agent:**
> I've searched your LearnUpon portal and found 'John Doe' (ID: 12345). He is currently active and has 3 active enrollments. Would you like to see his course progress?

---

**👤 You:**
> "Search for courses related to 'Cybersecurity'."

**🤖 AI Agent:**
> I found 2 courses matching 'Cybersecurity': 'Introduction to Cybersecurity' (ID: 101) and 'Advanced Threat Detection' (ID: 102).

---

**👤 You:**
> "Enroll user ID '12345' into course ID '101'."

**🤖 AI Agent:**
> Successfully enrolled user 12345 into 'Introduction to Cybersecurity'. The new enrollment ID is '98765'.


## Installation & Usage

To install and use the **LearnUpon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/learnupon](https://vinkius.com/mcp/learnupon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
