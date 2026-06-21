# Learn Amp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/learn-amp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/learn-amp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/learn-amp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Combine learning, engagement, and performance in one people development platform that helps employees grow and organizations thrive.

## Description
Connect your **Learn Amp** organizational account to any AI agent and take full control of your learning and development workflows through natural conversation.

### What you can do

- **User Management** — List all users, create new accounts, and manage profile data across your organization.
- **Content & Courses** — Query the complete library of learning items, documents, and interactive courses.
- **Learning Pathways** — List and inspect Learnlists to understand curated employee development tracks.
- **Progress Tracking** — Mark items as complete and monitor engagement verbs across the platform.
- **Access Control** — Deactivate or reactivate user accounts to maintain a secure and up-to-date directory.

### How it works

1. Subscribe to this server
2. Enter your Learn Amp Client ID and Client Secret
3. Start managing your L&D ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **L&D Managers** — instantly retrieve course lists, check user progress, and manage enrollments without opening the dashboard.
- **HR & Operations** — automate user provisioning and deactivation during onboarding and offboarding flows.
- **Team Leads** — verify skill development and course completion metrics for your direct reports via AI.


## Available Tools
- **complete_item**: Mark a learning item as complete for a user
- **create_user**: Create a new user in Learn Amp
- **deactivate_user**: The user data remains but they can no longer log in.

Deactivate a user account
- **get_learnlist**: Get details for a specific learnlist
- **get_user**: Get details for a specific user
- **list_items**: List all learning items (courses, content)
- **list_learnlists**: List all learnlists (learning pathways)
- **list_users**: List all users from Learn Amp
- **list_verbs**: List all available action verbs
- **update_user**: Update an existing user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Learn Amp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in my Learn Amp account."

**🤖 AI Agent:**
> I've fetched your user directory. You have 42 active users including 'Alex Rivera' and 'Sarah Chen'. Would you like to check the learning progress for any of them?

---

**👤 You:**
> "Show me all available courses related to 'Compliance'."

**🤖 AI Agent:**
> Searching the library... I found 3 items: 'GDPR Basics', 'Cybersecurity 101', and 'Annual Ethics Training'. Which one would you like to inspect?

---

**👤 You:**
> "Mark course 8823 as completed for user 1029."

**🤖 AI Agent:**
> Processing completion... Done! Item 8823 has been successfully marked as completed for user 1029. Their progress has been updated in the system.


## Installation & Usage

To install and use the **Learn Amp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/learn-amp](https://vinkius.com/mcp/learn-amp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
