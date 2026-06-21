# Checkr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate background checks via Checkr — screen candidates, monitor reports, and manage compliance directly from any AI agent.

## Description
Connect your **Checkr** account to any AI agent and take full control of your background screening and hiring compliance through natural conversation. Streamline how you screen candidates and verify credentials.

### What you can do

- **Candidate Oversight** — List and retrieve details for all candidates in your account natively
- **Report Intelligence** — Access background check reports and their current status (Clear, Consider, Pending) flawlessly
- **Screening Automation** — Create new candidate profiles and initiate background checks securely
- **Package Logistics** — List and manage available screening packages like 'Pro' and 'Basic' flawlessly
- **Invitation Control** — Monitor invitations sent to candidates to complete their own screening applications securely
- **Compliance Monitoring** — Retrieve detailed report results and adverse action status directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkr API Secret Key (obtained from your dashboard)
3. Start managing your background checks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — monitor background check progress and review candidate statuses using natural language
- **Recruiters** — create new candidates and trigger screenings without opening the dashboard
- **Compliance Officers** — audit report results and verify screening packages straight from their chat interface
- **Operations Teams** — quickly check the status of pending invitations and candidate profiles


## Available Tools
- **create_new_candidate**: Create a new candidate profile
- **start_background_check**: Initiate a background check for a candidate
- **get_candidate_details**: Get detailed information for a specific candidate
- **get_report_details**: Get detailed information for a specific background report
- **list_checkr_candidates**: List candidates in the account
- **list_screening_invitations**: List invitations sent to candidates
- **list_screening_packages**: List available screening packages (e.g. Pro, Basic)
- **list_background_reports**: List background check reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 background checks in my Checkr account."

**🤖 AI Agent:**
> Retrieving recent reports... I found 5 items: John Doe (Clear), Jane Smith (Pending), Mike Miller (Consider), and 2 others. Would you like to see the details for Mike Miller?

---

**👤 You:**
> "Check the status of the candidate named 'Jane Smith'."

**🤖 AI Agent:**
> Searching for Jane Smith... I found 1 profile. Her background check is currently 'Pending' (75% complete). We are waiting for the motor vehicle record check to finish.

---

**👤 You:**
> "What screening packages do I have available?"

**🤖 AI Agent:**
> Checking your available packages... You have 3 configured: 'Standard Pro' (Criminal + MVR), 'Basic' (Criminal Only), and 'Executive' (Standard + Credit + Employment).


## Installation & Usage

To install and use the **Checkr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkr](https://vinkius.com/mcp/checkr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
