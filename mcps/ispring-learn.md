# iSpring Learn MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ispring-learn)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ispring-learn-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ispring-learn-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Train employees with a corporate LMS that delivers SCORM courses, tracks certifications, and generates compliance reports.

## Description
Connect your **iSpring Learn** instance to any AI agent and manage training through natural conversation.

### What you can do

- **Course Catalog** — Browse all courses with enrollment counts and completion rates
- **Learner Management** — List learners, inspect profiles, and track individual progress
- **Enrollment Tracking** — Monitor who is enrolled in which courses
- **Quiz Results** — Review quiz scores and assessment outcomes
- **Completion Reports** — Track overall training completion metrics
- **Department Access** — Browse organizational structure for targeted training

### How it works

1. Subscribe to this server
2. Enter your iSpring Learn account URL and API Key
3. Start managing training from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **L&D Teams** — monitor training progress and completion rates
- **HR Managers** — track compliance training and enrollment
- **Training Coordinators** — review quiz results and learner performance


## Available Tools
- **create_new_learner**: Register a new user
- **get_course_details**: Get details for a specific course
- **get_learning_report**: Get training report
- **list_learning_courses**: List LMS courses
- **list_course_enrollments**: List course enrollments
- **list_user_groups**: List organizational groups
- **list_learners**: List iSpring Learn users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iSpring Learn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all courses with completion rates and learners falling behind."

**🤖 AI Agent:**
> Courses: 8 active. 'Cybersecurity Essentials' (45 enrolled, 78% complete). 'Onboarding 2025' (12 enrolled, 92%). 'GDPR Compliance' (60 enrolled, 65% ⚠️). 'Sales Training' (20 enrolled, 85%). Falling behind (< 30% in required courses): 5 learners in GDPR, 2 in Cybersecurity. Deadline: May 1.

---

**👤 You:**
> "Show quiz results for the Cybersecurity course and the top performers."

**🤖 AI Agent:**
> Cybersecurity quiz: 38 attempts. Pass rate: 82%. Average score: 78/100. Top: Sarah Chen (98/100), Mike Torres (95/100), Lisa Park (92/100). Failed: 7 learners (avg 45/100). Most missed question: 'Phishing identification' (34% correct). Would you like to see individual learner details?

---

**👤 You:**
> "List all departments and their training completion status."

**🤖 AI Agent:**
> Departments: 6. Engineering (12 people, 89% complete). Product (4, 95%). Design (3, 100% ✅). Marketing (5, 72% ⚠️). Sales (8, 81%). HR (3, 100% ✅). Overall: 35 employees, 85% average completion. Marketing needs attention: 2 learners haven't started GDPR.


## Installation & Usage

To install and use the **iSpring Learn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ispring-learn](https://vinkius.com/mcp/ispring-learn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
