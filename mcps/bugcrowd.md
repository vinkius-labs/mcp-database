# Bugcrowd MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugcrowd)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bugcrowd-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bugcrowd-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage crowdsourced security via Bugcrowd — track submissions, programs, and targets directly from any AI agent.

## Description
Connect your **Bugcrowd** account to any AI agent and orchestrate your vulnerability management, bug bounty programs, and security engagements through natural conversation.

### What you can do

- **Submission Oversight** — List and retrieve detailed metadata for all vulnerability reports (submissions) across your programs.
- **Program Management** — List all active security programs and retrieve detailed metadata, including scopes and rewards.
- **Engagement Tracking** — Monitor crowd executions like specific Bug Bounties or Pen Tests directly from your workspace.
- **Target Coordination** — List and inspect assets in scope (targets) for your organization or specific programs.
- **Submission Creation** — Create new vulnerability submissions from external sources using natural language.
- **Organizational Insights** — Retrieve core organization information and settings straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Bugcrowd API Access Token
3. Start managing your crowdsourced security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers & Analysts** — quickly check submission statuses or program scopes without manual dashboard work.
- **Vulnerability Managers** — retrieve and triage reports straight from their workflow tools.
- **CisOs & Security Leads** — monitor program health and target coverage using natural language.


## Available Tools
- **create_submission**: Create a new vulnerability submission
- **get_engagement**: Get details of a specific engagement
- **get_organization_info**: Retrieve core organization information
- **get_program**: Get details of a specific security program
- **get_submission**: Get details of a specific submission
- **get_target**: Get details of a specific target
- **list_engagements**: List all crowd engagements (bounties, pen tests)
- **list_programs**: List all security programs
- **list_submissions**: List all vulnerability submissions
- **list_targets**: List all assets in scope (targets)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bugcrowd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active security programs in Bugcrowd."

**🤖 AI Agent:**
> I've retrieved your programs. You have 3 active programs: 'Vinkius Bounty' (ID: prog_1), 'Main Web App' (ID: prog_2), and 'Legacy Systems' (ID: prog_3).

---

**👤 You:**
> "Show the last 5 vulnerability submissions."

**🤖 AI Agent:**
> Retrieving submissions... Your 5 most recent reports include 'SQL Injection in /api' (Triaged), 'XSS on Login Page' (Unresolved), and 'Broken Auth' (Resolved).

---

**👤 You:**
> "Create a new submission titled 'Insecure Direct Object Reference' for program prog_123."

**🤖 AI Agent:**
> Submission 'Insecure Direct Object Reference' has been successfully created for program prog_123 with ID sub_99283.


## Installation & Usage

To install and use the **Bugcrowd** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugcrowd](https://vinkius.com/mcp/bugcrowd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
