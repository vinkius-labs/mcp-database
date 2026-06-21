# 360Learning MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/360learning)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/360learning-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/360learning-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collaborative learning platform — manage users, courses, paths, and training statistics via AI.

## Description
Empower your corporate education strategy with **360Learning**, the collaborative learning platform now fully integrated with your AI agent. By connecting 360Learning via the Model Context Protocol, you transform learning management from a complex administrative task into a natural conversation. Your agent can now seamlessly provision learners, audit course completions, and retrieve real-time training statistics without you ever navigating a LMS dashboard. It’s the smartest way to scale knowledge sharing and ensure your team stays ahead of the curve.

### What you can do

- **User Management** — List, create, and update learners and admins within your platform.
- **Course Catalog** — Browse available courses, view lesson details, and check enrollment status.
- **Learning Paths** — Manage structured training paths and monitor group progress across curriculum.
- **Engagement Stats** — Access completion rates, time spent, and assessment scores to gauge training effectiveness.
- **Group Organization** — List and manage departments or training cohorts for targeted learning delivery.

### How it works

1. Subscribe to this server
2. Enter your 360Learning API Key and Company ID
3. Start managing your collaborative learning environment through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **L&D Professionals** — automate training reports and user provisioning effortlessly
- **HR Managers** — monitor onboarding progress and mandatory compliance training
- **Team Leaders** — check team skill gaps and course completion status on the fly
- **Internal Trainers** — manage course materials and learner feedback through simple commands


## Available Tools
- **list_users**: Use this to find specific learner profiles.

List all active learners and administrators in the 360Learning platform
- **create_user**: Requires the email, first name, and last name of the user.

Register a new learner, author, or administrator account
- **list_courses**: Use this to find a specific Course ID to check enrollments or detailed lessons.

Browse the catalog of available training courses
- **get_course**: Get technical details and the lesson overview for a specific course
- **get_stats**: You must filter by either Group ID, User ID, or Course ID.

Retrieve training completion rates and assessment scores
- **list_groups**: Useful for finding a specific Group ID for reporting strategies.

List all training groups, departments, or cohorts in the platform


## 💬 Prompt Examples

Here are some examples of how you can interact with the **360Learning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in my 360Learning platform."

**🤖 AI Agent:**
> I've retrieved the list of active users. You have 150 learners and 5 admins currently registered. Would you like to see details for a specific user?

---

**👤 You:**
> "Show me the training statistics for the 'Marketing' group."

**🤖 AI Agent:**
> I've compiled the training stats for the Marketing group. The average completion rate is 82% with an average assessment score of 88. Would you like a list of users who haven't finished their courses?

---

**👤 You:**
> "List all available courses in the catalog."

**🤖 AI Agent:**
> I've retrieved the 360Learning course catalog. You have 24 active courses, including 'Onboarding 2024' and 'Advanced Sales Techniques'. Which one would you like to explore in detail?


## Installation & Usage

To install and use the **360Learning** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/360learning](https://vinkius.com/mcp/360learning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
