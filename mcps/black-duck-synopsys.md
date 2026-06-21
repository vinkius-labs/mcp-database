# Black Duck (Synopsys) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/black-duck-synopsys)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/black-duck-synopsys-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/black-duck-synopsys-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Secure your open source supply chain via Black Duck — list projects, versions, and vulnerabilities directly from any AI agent.

## Description
Connect your **Black Duck (Synopsys)** instance to any AI agent and orchestrate your open source security and license compliance workflows through natural conversation.

### What you can do

- **Project Oversight** — List and retrieve detailed metadata for all your software projects and their versions.
- **Vulnerability Tracking** — Query project versions for known vulnerabilities (CVEs) and retrieve severity levels.
- **BOM Monitoring** — Check the status of Bill of Materials (BOM) calculations to ensure up-to-date compliance data.
- **Policy Management** — List and audit security policy rules defined across your organization.
- **Scan Analysis** — Access code locations and scan histories to track security coverage.
- **User & Access Auditing** — Retrieve user profiles and manage access controls within the platform.

### How it works

1. Subscribe to this server
2. Enter your Black Duck Instance URL and API Token
3. Start securing your code from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — quickly audit vulnerabilities across multiple projects without manual dashboard exports.
- **Developers** — check the security status of their project dependencies straight from the code editor.
- **Compliance Officers** — retrieve policy rule summaries and BOM statuses for periodic reporting.


## Available Tools
- **get_bom_status**: Check BOM calculation status for a project version
- **get_project**: Get details of a specific project
- **list_vulnerabilities**: List vulnerabilities for a project version
- **get_vulnerability_details**: Get details of a specific CVE/Vulnerability
- **list_code_locations**: List all scan code locations
- **list_policy_rules**: List all security policy rules
- **list_project_versions**: List all versions for a specific project
- **list_projects**: List all Black Duck projects
- **list_users**: List all Black Duck users
- **search_projects**: Search projects by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Black Duck (Synopsys)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all versions for project 'Web-Portal'."

**🤖 AI Agent:**
> I've retrieved the versions for 'Web-Portal'. You have 3 versions: '1.0.0' (ID: v1), '1.1.0-beta' (ID: v2), and 'latest' (ID: v3).

---

**👤 You:**
> "Identify any critical vulnerabilities in the backend service repository."

**🤖 AI Agent:**
> Scanning project 'Backend Service'. Found 2 Critical CVEs linked to active OpenSSL dependencies (CVE-2023-xxxx). Actions recommended immediately.

---

**👤 You:**
> "Fetch the BOM status for project Alpha version 2.0."

**🤖 AI Agent:**
> The Bill of Materials (BOM) for Alpha v2.0 is perfectly 'UP_TO_DATE' and fully synchronized within the compliance policy guidelines.


## Installation & Usage

To install and use the **Black Duck (Synopsys)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/black-duck-synopsys](https://vinkius.com/mcp/black-duck-synopsys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
