# Innform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/innform-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/innform-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/innform-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Train your team with an LMS that creates courses from your content, tracks completion, and gamifies the learning experience.

## Description
Connect your **Innform** training portal to any AI agent and take full control of your Learning Management System (LMS) and employee compliance workflows through natural conversation.

### What you can do

- **User Lifecycle Orchestration** — List all learners and admins, retrieve detailed high-fidelity profile metadata, and invite new users programmatically
- **Assignment Intelligence** — Programmatically monitor completed and overdue training assignments to maintain a perfectly coordinated compliance overview
- **Training Group Architecture** — Access your complete directory of learner groups and their properties to oversee your organizational training structure
- **Access Control Management** — Programmatically freeze or unfreeze learner accounts to manage platform access dynamically based on organizational needs
- **Operational Monitoring** — Verify API connectivity and monitor training progress directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Innform dashboard (Account Settings > Integrations)
3. Start orchestrating your training ecosystem from Claude, Cursor, or any MCP client

No more manual checking of individual progress bars or digging through CSV reports. Your AI acts as your dedicated training coordinator and compliance architect.

### Who is this for?

- **L&D Managers** — instantly retrieve training completion recaps and manage user access using natural language commands
- **Compliance Officers** — monitor overdue assignments and verify team progress without leaving your workspace
- **HR Operations** — automate the onboarding of new learners into specific groups through simple AI queries


## Available Tools
- **freeze_user**: Freeze a user account
- **get_user_details**: Get details for a specific user
- **invite_user**: Invite a new learner
- **list_completed_assignments**: List completed training assignments
- **list_groups**: List learner groups
- **list_overdue_assignments**: List overdue training assignments
- **list_users**: List Innform users
- **unfreeze_user**: Unfreeze a user account
- **update_user**: Update an existing user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Innform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active learners in my Innform portal."

**🤖 AI Agent:**
> I've retrieved your learners. You currently have 50 active users, including 'Jane Smith' and 'John Doe'. Would you like the detailed high-fidelity metadata for any of them?

---

**👤 You:**
> "Show me all overdue training assignments for the Engineering team."

**🤖 AI Agent:**
> Accessing compliance data... I found 5 overdue assignments in Engineering, including 'Security 101'. I've retrieved the high-fidelity overdue dates for your review. Need help notifying these users?

---

**👤 You:**
> "Freeze account for learner ID 'user_123' immediately."

**🤖 AI Agent:**
> Access orchestrated! I've successfully frozen the account for user_123. They will no longer be able to access the training portal until unfrozen. Need help managing other account statuses?


## Installation & Usage

To install and use the **Innform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/innform-alternative](https://vinkius.com/mcp/innform-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
