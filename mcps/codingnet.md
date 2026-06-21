# Coding.net MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/codingnet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/codingnet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/codingnet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

All-in-one DevOps platform — manage projects, repositories, and issues via AI.

## Description
Empower your AI agent to orchestrate your entire software development lifecycle with **CODING** (Coding.net), the premier DevOps platform in China. By connecting CODING to your agent, you transform complex project management, code repository auditing, and issue tracking into a natural conversation. Your agent can instantly list projects, retrieve detailed Git repository metadata, browse active merge requests, and monitor issue progress without you ever needing to navigate the comprehensive CODING web interface. Whether you are conducting a code review or coordinating a cross-functional release, your agent acts as a real-time DevOps assistant, keeping your development data accurate and your team moving.

### What you can do

- **Project Orchestration** — List all DevOps projects and retrieve detailed metadata for each organizational unit.
- **Repository Auditing** — Browse Git depots, list branches, and retrieve detailed commit information.
- **Issue Tracking** — List and retrieve detailed information about project tasks and bugs to monitor velocity.
- **Collaboration Monitoring** — List active merge requests to identify blockers and pending reviews.
- **User Insights** — Retrieve profile information for organization members and the authenticated user.

### How it works

1. Subscribe to this server
2. Enter your CODING Team Domain and Personal Access Token
3. Start managing your DevOps lifecycle through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate repository auditing and monitor CI/CD pipelines through natural language.
- **Project Managers** — track issue progress and monitor team velocity directly from your AI-powered workspace.
- **Engineering Leads** — coordinate code reviews and browse merge requests via a unified AI interface.
- **CODING Power Users** — integrate your existing DevOps workflows into your AI-driven daily routines.


## Available Tools
- **get_commit**: Get commit details
- **get_issue**: Get issue details
- **get_project**: Get project details
- **get_repo**: Get repository details
- **get_user**: Get current user profile
- **list_branches**: List repository branches
- **list_issues**: List project issues
- **list_mrs**: List merge requests
- **list_projects**: List DevOps projects
- **list_repos**: List project repositories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coding.net** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my DevOps projects on CODING."

**🤖 AI Agent:**
> I've retrieved your CODING projects. You have 5 active projects, including 'E-commerce Backend', 'Mobile App', and 'Infrastructure'. Which one would you like to explore?

---

**👤 You:**
> "Show me the latest issues for project 'Alpha'."

**🤖 AI Agent:**
> I've listed the latest issues for project 'Alpha'. There are 12 open tasks, including 'Bug: Login Timeout' and 'Feature: Dark Mode'. Would you like the details for the high-priority ones?

---

**👤 You:**
> "Get the branches for repository 'main-api' in project 'Alpha'."

**🤖 AI Agent:**
> I've retrieved the branches for 'main-api'. You have 3 active branches: 'master', 'develop', and 'feature/api-v2'. Should I check for the latest commit on any of them?


## Installation & Usage

To install and use the **Coding.net** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codingnet](https://vinkius.com/mcp/codingnet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
