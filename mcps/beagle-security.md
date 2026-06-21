# Beagle Security MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beagle-security)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/beagle-security-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/beagle-security-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate security testing via Beagle Security — list projects, start tests, and retrieve results directly from any AI agent.

## Description
Connect your **Beagle Security** account to any AI agent and integrate automated penetration testing into your development workflow through natural conversation.

### What you can do

- **Project Oversight** — List and manage all security projects and target applications.
- **On-Demand Testing** — Trigger new security tests for your applications instantly.
- **Status Monitoring** — Check the real-time progress of ongoing security assessments.
- **Vulnerability Retrieval** — Access detailed results and lists of vulnerabilities found during tests.
- **Compliance & Auditing** — Retrieve account profiles and test histories for compliance reporting.

### How it works

1. Subscribe to this server
2. Enter your **Personal Access Token** and your **Application Token** — both are required
3. Start managing your application security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate the triggering of tests and retrieval of findings without manual dashboard navigation.
- **Developers** — check security test status and results straight from the code editor.
- **DevSecOps Teams** — integrate security testing into automated CI/CD summaries and agent-led workflows.


## Available Tools
- **get_application_details**: Get details of an application
- **get_project_details**: Get details of a specific project
- **get_test_results**: Retrieve security test results
- **get_test_status**: Check status of a security test
- **get_user_profile**: Get Beagle account profile
- **get_vulnerabilities**: List vulnerabilities for a test
- **list_applications**: List security applications
- **list_projects**: List Beagle Security projects
- **start_test**: Start a new security test
- **stop_test**: Stop an active security test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beagle Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current security projects on Beagle."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 3 projects: 'E-commerce API' (ID: proj_123), 'Mobile Backend' (ID: proj_456), and 'Admin Dashboard' (ID: proj_789). Which one would you like to inspect?

---

**👤 You:**
> "Start a new security test for application token app_998877."

**🤖 AI Agent:**
> Triggering the security test... Done! Test ID 'test_554433' has been started for your application. You can check its status using `get_test_status`.

---

**👤 You:**
> "Show me the findings from the last test test_554433."

**🤖 AI Agent:**
> Retrieving results for test_554433... I found 3 vulnerabilities: 1 Critical (SQL Injection), 1 High (XSS), and 1 Medium (Missing Security Headers). Would you like the full details for the SQL Injection?


## Installation & Usage

To install and use the **Beagle Security** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beagle-security](https://vinkius.com/mcp/beagle-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
