# HackEDU (Security Journey) MCP Server

Automate security training via HackEDU — manage users, track progress, and integrate vulnerability data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hackedu-security-journey)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **HackEDU** (now part of Security Journey) platform to any AI agent and take full control of your secure coding training workflows through natural conversation.

### What you can do

- **User & Team Management** — List all users and teams, retrieve detailed profiles, and check UUIDs for assignments.
- **Progress Tracking** — Monitor individual and team training progress to ensure security compliance across your organization.
- **Content Insights** — Browse the full catalog of available security training modules and lessons.
- **Vulnerability Integration** — Access HackEDU’s vulnerability taxonomy mapped to CWE, CVE, and CAPEC standards.
- **Adaptive Training** — Push issues from bug bounty programs or scanners to trigger personalized training plans for developers.
- **Reporting** — Instantly retrieve summaries of security training health and identifying gaps in developer knowledge.

### How it works

1. Subscribe to this server
2. Enter your HackEDU API Key (from the Admin Dashboard)
3. Start managing your security training from Claude, Cursor, or any MCP-compatible client

No more manual exporting of training reports. Your AI assistant acts as a dedicated Security Program Manager or AppSec Coordinator.

### Who is this for?

- **Security Engineers** — instantly retrieve training statuses and sync vulnerability findings to trigger adaptive lessons.
- **Engineering Managers** — track team progress and identify top security performers or areas needing improvement.
- **AppSec Teams** — automate the integration of bug bounty data into developer training flows.


## Available Tools
- **create_issue**: Create/Push a new vulnerability issue to trigger adaptive training
- **get_team_progress**: Get the training progress for a specific team
- **get_user**: Get detailed information about a specific user
- **get_user_progress**: Get the training progress for a specific user
- **list_adaptive_training_plans**: List adaptive training plans created based on vulnerability findings
- **list_content**: List all available training modules and lessons
- **list_issues**: List vulnerability issues synced from external sources (e.g., Bugcrowd, HackerOne)
- **list_teams**: List all teams configured in HackEDU
- **list_users**: List all users in your HackEDU account
- **list_vulnerabilities**: List HackEDU vulnerability taxonomy (CWE/CVE/CAPEC mapping)


## Installation & Usage

To install and use the **HackEDU (Security Journey)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hackedu-security-journey](https://vinkius.com/mcp/hackedu-security-journey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
