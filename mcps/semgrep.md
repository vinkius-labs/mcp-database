# Semgrep MCP Server

Equip your AI agent with read/write access to Semgrep's SAST platform to audit code security findings, update triage statuses, and enforce custom semantic rules.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/semgrep)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect the **Semgrep** AppSec platform directly to your AI agent to radically accelerate code security triaging. Instead of forcing developers to jump between their IDE and the Semgrep dashboard, empower your AI to pull 'Findings', analyze the vulnerable syntax, and instantly close false positives.

### What you can do

- **Triage Findings (Bugs)** — Instruct the agent to grab the latest CI vulnerability findings and immediately push a status update to mark it as fixed, ignored, or mitigated (`update_finding_status`)
- **Rule Management** — Request the AI to look at a newly discovered bad coding pattern and command it to write and deploy a matching custom semantic rule (`create_rule`) to your organizational deployment
- **Project & Deployment Scoping** — Map out all repositories running Semgrep actions and check their overarching security health scores in milliseconds
- **Comprehensive Forensics** — Fetch granular SCA and SAST semantic flaw definitions, including exact snippets, CVE links, and the specific bad lines causing the trigger

### How it works

1. Enable this MCP server within your workflow
2. Supply a standard API Token from your Semgrep Dashboard settings
3. Engage your agent in Cursor or Claude to cross-examine security warnings dynamically

### Who is this for?

- **Security Engineers (AppSec)** — tell the AI to quickly delete an obsolete rule across the entire deployment without wrestling with the dashboard interface
- **DevOps** — retrieve compliance metrics and pipeline fix rates natively and pipe them directly into an executive summary report via chat
- **Software Developers** — let Cursor fetch the specific `finding_id` blocking your PR, explain what the vulnerability means, and draft the exact semantic fix to pass the scan


## Available Tools
- **create_rule**: Allows developers to forbid project-specific bad patterns securely and continuously across the enterprise repositories.

Create a customized Semgrep security rule within the platform
- **delete_rule**: Delete a custom Semgrep security rule from the deployment
- **list_deployments**: The primary key is the deployment slug identifier. Almost all subsequent API operations targeting rules, projects, or findings will require this deployment slug to define the scope.

List Semgrep organizational deployments
- **list_findings**: Findings provide snippet details, file line numbers, severity, and rule types.

Fetch global static analysis security findings for a deployment
- **get_finding_details**: Explains the exact malicious code block, suggests semantic fixes, states whether it is blocking PRs in CI, and links to CVE data (if an SCA supply chain defect).

Get atomic details for a specific Semgrep flaw
- **get_project**: Search for a precise Semgrep project by exact repository name
- **list_rules**: The rules are structured YAML definitions that search for semantic anti-patterns in codebases (e.g., unparameterized SQL queries, hardcoded AWS keys).

List Semgrep semantic rules deployed globally
- **get_metrics**: Typically consumed to render executive security dashboards.

Get AppSec metrics and compliance stats for Semgrep
- **list_projects**: Projects maintain a link between developers and static security scan outputs over time.

List Semgrep projects (repositories) monitored in a deployment
- **update_finding_status**: Valid states generally include active, fixed, false_positive, ignored, mitigated. Resolving findings through this API cleans up the developer experience when managing compliance queues.

Mark a Semgrep finding state (e.g., fixed, false positive)


## Installation & Usage

To install and use the **Semgrep** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semgrep](https://vinkius.com/mcp/semgrep)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
