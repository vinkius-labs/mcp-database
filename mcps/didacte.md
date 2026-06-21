# Didacte MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/didacte)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/didacte-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/didacte-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to manage LMS courses, track learner progress, and monitor enrollments via the Didacte (Workleap) API.

## Description
Integrate **Didacte** (by **Workleap**), the powerful and user-friendly learning management system (LMS), directly into your AI workflow. Manage your course catalog, monitor student enrollments and real-time progress, and audit your organization's learning activity using natural language.

### What you can do

- **Course Oversight** — List and retrieve detailed configuration for all courses available in your Didacte portal.
- **Learner Intelligence** — Access detailed profiles for users and track their learning history across the organization.
- **Progress Tracking** — Monitor individual enrollment progress and identify active learners in real-time.
- **Curriculum Research** — List lessons and modules within courses to understand the learning structure and content.

### How it works

1. Connect the Didacte integration to your AI assistant.
2. Authorize using your Didacte API Token and portal Subdomain.
3. Orchestrate your corporate training and online learning through intuitive conversation.

### Who is this for?

- **L&D Professionals** — Quickly check enrollment numbers and learner progress on the go.
- **Training Coordinators** — Research user profiles and course curricula via chat.
- **Hiring & Onboarding Teams** — Monitor progress of new hire training plans and certifications instantly.


## Available Tools
- **get_account_metadata**: Retrieve metadata and usage limits for your Didacte organization
- **get_course_details**: Get detailed settings and information for a specific course
- **get_user_learning_profile**: Get full profile and summary for a specific user
- **list_active_learning_progress**: Identify enrollments where learners have made recent progress (mock logic)
- **list_course_enrollments**: List all users currently enrolled in a specific course
- **list_lms_courses**: List all available courses in your Didacte organization
- **list_user_enrollments**: List all courses a specific user is enrolled in
- **list_course_curriculum**: List all lessons and modules within a specific course
- **list_organization_users**: List all users and learners registered in your organization
- **search_courses_by_title**: Search for a course using a title keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Didacte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active courses in our portal."

**🤖 AI Agent:**
> I've found 12 active courses, including 'Company Compliance 2024', 'Advanced Project Management', and 'Security Awareness'. Would you like to see the enrollment count for any of these?

---

**👤 You:**
> "What is the progress for user 'Alice Johnson' in the 'Compliance' course?"

**🤖 AI Agent:**
> Alice Johnson has completed 75% of the 'Company Compliance 2024' course. She has 2 lessons remaining. Should I check if she has any other pending enrollments?

---

**👤 You:**
> "Search for courses related to 'Leadership'."

**🤖 AI Agent:**
> I've found 3 courses matching 'Leadership': 'New Manager Foundations', 'Effective Communication', and 'Strategic Decision Making'. Would you like a detailed curriculum for 'New Manager Foundations'?


## Installation & Usage

To install and use the **Didacte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/didacte](https://vinkius.com/mcp/didacte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
