# Snyk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snyk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snyk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snyk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Bring your Snyk code security ecosystem directly to your AI. Analyze vulnerabilities, project metadata, and scan issues right from your editor.

## Description
Connect your **Snyk** security dashboard natively to your preferred AI agent. Speed up your DevSecOps workflow by diagnosing and investigating package vulnerabilities via natural language. Rather than jumping between browser tabs trying to locate a specific CVE report, query your organizational vulnerability footprint dynamically through MCP.

### What you can do

- **Project Surveillance** — Discover application projects via `list_projects` and fetch internal configurations calling `get_project_details`
- **Vulnerability Hunting** — Expose specific codebase flaws instantly with `list_issues`, extracting actionable remediation steps querying `get_issue_details`
- **Company Operations** — Traverse hierarchical structures via `list_organizations` and see who contributes using `list_organization_members`
- **Admin Controls** — Monitor API connectivity invoking `list_integrations` and check scan caps via `get_usage_stats` and `get_billing_info`

### How it works

1. Subscribe to this AI integration server
2. Introduce your personal Snyk API Token
3. Start using Claude, Cursor, or your terminal IDE to command your security checks

Stop digging through the Snyk UI just to see why a container build failed. Find the precise faulty dependency versions instantly within your codebase context.

### Who is this for?

- **DevSecOps** — query exact details on critical CVEs before approving PR merges, generating threat analysis models quickly
- **App Developers** — discover which underlying package versions triggered build issues seamlessly without running local dependency scanners
- **SysAdmins** — pull quick organizational billing usage limits dynamically and audit user integrations from pure text instructions


## Available Tools
- **get_billing_info**: Retrieves billing details for an organization
- **get_issue_details**: Retrieves details for a specific security issue
- **get_project_details**: Retrieves details for a specific project
- **get_usage_stats**: Retrieves usage statistics
- **list_integrations**: Lists active integrations for an organization
- **list_issues**: Lists security issues for a specific project
- **list_organization_members**: Lists all members of a Snyk organization
- **list_organizations**: Lists all Snyk organizations
- **list_projects**: Lists all projects in a specific organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snyk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check Snyk and summarize all critical security vulnerabilities currently found in the main backend project."

**🤖 AI Agent:**
> I scanned 'Core Backend' (ID: `a1b2c3`) using the `list_issues` action path. You have **2 Critical Issues** flagged:

1. **Arbitrary File Write via Archive Extraction (Zip Slip)** - Found in `adm-zip@0.4.11` 
2. **Prototype Pollution** - Found in `lodash@4.17.15`

Would you like me to inspect 'Prototype Pollution' using `get_issue_details` to view the recommended fix paths?

---

**👤 You:**
> "Display our organization's current integration links on Snyk. What are we attached to?"

**🤖 AI Agent:**
> Triggering the `list_integrations` routine... 
Your organization (`org_123_abc`) has 3 active pipelines feeding into Snyk:
- **GitHub Enterprise** (Source Control)
- **AWS ECR** (Container Registry)
- **Slack** (Alert Hook Notification)

All connections appear functional on the organizational tier.

---

**👤 You:**
> "Draw a markdown table checking the team member roles in the DevOps organization."

**🤖 AI Agent:**
> I've pulled the organizational data through `list_organization_members` for the **DevOps Core** tenant:

| Member Name | Associated Email | Snyk Role |
| --- | --- | --- |
| Alex Mercer | a.mercer@company.co | `Admin` |
| Sarah Chen | s.chen@company.co | `Collaborator` |
| Marc Johnson | m.johnson@company.co | `Viewer` |

Total count: 3 members mapped directly.


## Installation & Usage

To install and use the **Snyk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snyk](https://vinkius.com/mcp/snyk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
