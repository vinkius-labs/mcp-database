# Coassemble MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coassemble)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coassemble-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coassemble-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage online training and LMS via Coassemble — track courses, monitor enrolments, and manage student groups directly from any AI agent.

## Description
Connect your **Coassemble** account to any AI agent and take full control of your online training and LMS through natural conversation. Streamline how you manage learners, courses, and completion results natively.

### What you can do

- **Course Oversight** — List and retrieve details for all training courses in your workspace natively
- **Enrolment Intelligence** — Access and monitor student enrolments and their current progress flawlessly
- **Member Management** — List all workspace members and their contact details securely
- **Group Logistics** — Monitor student groups and manage their course associations flawlessly
- **Completion Auditing** — Retrieve training results and grades for all enrolments to track success flawlessly
- **Profile Visibility** — Access your own user profile and core workspace metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Coassemble User ID and User Token (obtained from Settings > API)
3. Start managing your online training from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **L&D Managers** — monitor course completion rates and student engagement using natural language
- **Course Instructors** — review individual student progress and results without opening the LMS dashboard
- **HR Teams** — quickly look up member profiles and group memberships straight from their chat interface
- **Ops Teams** — verify enrolment status and monitor training throughput


## Available Tools
- **enroll_member_in_course**: Enroll a specific member into a course or group
- **get_course_training_details**: Get detailed information for a specific course
- **get_member_group_associations**: Get all groups a specific member belongs to
- **list_coassemble_courses**: List all training courses in the Coassemble workspace
- **list_coassemble_enrolments**: List all course enrolments
- **list_coassemble_groups**: List all student groups in the workspace
- **list_coassemble_members**: List all members (users) in the workspace
- **get_training_completion_results**: List training results and grades for enrolments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coassemble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all training courses in my Coassemble workspace."

**🤖 AI Agent:**
> Retrieving your courses... I found 8 active courses including 'Company Onboarding', 'Compliance 101', and 'Advanced Sales Training'. Which one would you like to see enrolments for?

---

**👤 You:**
> "Show me the progress for user 'STU_12345'."

**🤖 AI Agent:**
> Checking progress for user STU_12345... This student is enrolled in 3 courses. They have completed 'Compliance 101' (100%) and are at 45% for 'Advanced Sales'.

---

**👤 You:**
> "What are the latest completion results?"

**🤖 AI Agent:**
> Retrieving completion data... You had 12 new course completions today. The average grade is 92%, with 'Onboarding' having the highest success rate.


## Installation & Usage

To install and use the **Coassemble** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coassemble](https://vinkius.com/mcp/coassemble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
