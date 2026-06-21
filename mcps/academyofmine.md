# AcademyOfMine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/academyofmine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/academyofmine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/academyofmine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage AcademyOfMine LMS — orchestrate courses, register learners, and track enrollments directly from any AI agent.

## Description
Connect your AI agents to **AcademyOfMine (AOM)**, the all-in-one platform for training and compliance. This MCP provides 11 tools to automate course management, user registration, and enrollment workflows directly from your AI agent.

### What you can do

- **Course Orchestration** — List, create, and update courses and their curriculum structures without leaving your agent
- **Learner Management** — Register new users, retrieve detailed profile information, and manage instructor accounts
- **Enrollment Automation** — Enroll or remove students from courses programmatically based on business logic
- **Portal Configuration** — Access and monitor default portal settings and configurations for your LMS instance

### How it works

1. Subscribe to this server
2. Log in to your [**AcademyOfMine Admin Dashboard**](https://academyofmine.com/)
3. Navigate to **Settings > Integrations > API**
4. Generate your **API Key**
5. Identify your **Portal Subdomain** (e.g., `myportal` from `myportal.aomlms.com`)
6. Connect your account to Vurb to start managing your LMS automation.

### Who is this for?

- **Training Managers** — automate student onboarding and course assignment at scale
- **Operations Teams** — sync LMS data with external business systems through AI-driven workflows
- **Educators & Admins** — quickly retrieve course details and enrollment statuses via natural language


## Available Tools
- **create_course**: Create a new course profile
- **create_user**: Create a new user account
- **enroll_student**: Enroll a student in a course
- **get_course_curriculum**: Retrieve the curriculum structure of a course
- **get_course_details**: Get detailed information for a specific course
- **get_portal_settings**: Retrieve LMS portal default settings
- **get_user_details**: Get detailed information for a specific user
- **list_courses**: List all courses available in the LMS
- **list_users**: List learners and instructors in the portal
- **unenroll_student**: Remove a student from a course
- **update_course**: Update an existing course


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AcademyOfMine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active courses in my AcademyOfMine portal and show their IDs."

**🤖 AI Agent:**
> I've fetched your course catalog. You currently have 4 active courses: 'Sales Mastery' (ID: 101), 'Cybersecurity Essentials' (ID: 102), 'Leadership Foundations' (ID: 103), and 'Product Roadmap' (ID: 104). Which one would you like to enroll a student in?

---

**👤 You:**
> "Enroll student 'user_777' into course 'crs_101'."

**🤖 AI Agent:**
> Processing enrollment... Student 'user_777' has been successfully enrolled in 'Sales Mastery' (ID: crs_101). They will receive an automated invitation email from the LMS.

---

**👤 You:**
> "Show me the curriculum details for course 'crs_advanced'."

**🤖 AI Agent:**
> Retrieving curriculum... Course 'Advanced Management' (ID: crs_advanced) contains 5 modules: 1. Strategic Thinking, 2. Financial Modeling, 3. Team Leadership... Would you like the lesson list for the first module?


## Installation & Usage

To install and use the **AcademyOfMine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/academyofmine](https://vinkius.com/mcp/academyofmine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
