# Yodiz MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yodiz)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yodiz-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yodiz-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage user stories, sprints, bugs, and epics on Yodiz — the all-in-one agile project management and issue tracking tool.

## Description
Connect your **Yodiz** account to any AI agent and manage your agile development lifecycle through natural conversation.

### What you can do

- **Requirement Tracking** — List and browse user stories within your projects to monitor requirements and backlog items
- **Release Management** — Browse all sprints (iterations) and retrieve sprint IDs to monitor release timelines and progress
- **Defect Monitoring** — List and track bugs and technical debt items for any specific project ID to ensure software quality
- **Roadmap Planning** — Access epics to see the macro-level roadmap and strategic business goals directly from your agent
- **Project Discovery** — List all agile projects and workspaces to retrieve numeric IDs for granular task management
- **Team Directory** — List all registered users in your workspace to find colleague IDs for task assignment and mentions
- **Agile Insights** — Quickly surface high-level features and iteration details required for automated project reporting

### How it works

1. Subscribe to this server
2. Enter your Yodiz API Key, Email, and Password
3. Start managing your agile backlog through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex agile boards to check a sprint status. Your AI agent becomes your agile project coordinator.

### Who is this for?

- **Scrum Masters & Agile Coaches** — monitor sprint progress and audit backlog items through simple chat commands
- **Product Owners** — quickly surface user stories and epic details to align with strategic roadmaps
- **QA Engineers** — track bugs and technical debt items across different projects without manual filtering
- **Development Teams** — lookup task details and team member IDs for faster collaboration


## Available Tools
- **list_projects**: Lists all agile projects in the Yodiz account
- **list_user_stories**: Provide the numeric project ID.

Lists user stories for a specific Yodiz project
- **list_sprints**: Lists all sprints (iterations) for a specific project
- **list_bugs**: Lists bugs and issues for a specific project
- **list_epics**: Lists epics (high-level features) for a project
- **list_users**: Lists all registered users in the Yodiz workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yodiz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Yodiz."

**🤖 AI Agent:**
> I found 4 active agile projects: 1. 'Cloud Infrastructure v2' (ID: 101), 2. 'Mobile App Redesign' (ID: 102), 3. 'API Gateway' (ID: 103), and 4. 'Internal Tooling' (ID: 104). Which one would you like to review?

---

**👤 You:**
> "Show me the user stories for project ID 102."

**🤖 AI Agent:**
> Retrieving stories for project 102... I found 12 items. Top items: 1. 'User Login with SSO' (Status: In Progress), 2. 'Add dark mode support' (Status: Backlog), 3. 'Optimize image loading' (Status: Done). Would you like the full details for any of these?

---

**👤 You:**
> "What sprints are scheduled for project ID 101?"

**🤖 AI Agent:**
> Project 101 has 3 scheduled iterations: 1. 'Sprint 24 - Networking' (Current), 2. 'Sprint 25 - Security Audit' (Upcoming), and 3. 'Sprint 26 - Scalability' (Future). Would you like to see the start and end dates for these sprints?


## Installation & Usage

To install and use the **Yodiz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yodiz](https://vinkius.com/mcp/yodiz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
