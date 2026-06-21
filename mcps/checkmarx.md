# Checkmarx MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkmarx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkmarx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkmarx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate AppSec via Checkmarx One — trigger core scans, analyze vulnerabilities, discover Best Fix Locations (BFL), and monitor KICS results.

## Description
Connect your **Checkmarx One** enterprise environment to any AI agent and take programmatic control over your Application Security posture. Analyze deep code flaws through natural chat instead of navigating complex cyber dashboards.

### What you can do

- **Projects & Applications** — Inventory your codebase containers, inspect active project linkages, and prepare specific branches for security scanning
- **Scans Lifecycle** — Trigger dynamic SAST/SCA security scans on repos, cancel redundant queues, and poll engines for precise execution timing
- **Vulnerability Triage** — Extract core datasets of severe vulnerabilities, mapping exact lines of code where the flawed logic resides
- **Best Fix Location (BFL)** — Ask the agent to calculate the exact optimal spot in your execution path to apply a patch that resolves the flaw entirely
- **KICS (IaC)** — Read specialized Infrastructure as Code metrics isolating misconfigurations exclusively in Terraform, Dockerfiles, or Kubernetes YAML

### How it works

1. Subscribe to this server
2. Provide your Checkmarx One JWT Token
3. Uncover code vulnerabilities natively inside Claude, Cursor, or any compatible MCP agent

### Who is this for?

- **Security Engineers (AppSec)** — seamlessly orchestrate vulnerability triage without toggling away from your primary workstation or ticket tracker
- **DevOps & Platform Teams** — investigate misconfigured KICS results in staging branches actively through the agent before deploying
- **Developers** — grab the exact Best Fix Location (BFL) for a zero-day issue and ask the LLM to rewrite the sanitization logic instantly


## Available Tools
- **cancel_scan**: Prevents unnecessary engine resource consumption and drops the scanning context if the developer pushed a new commit overlapping the running job.

Cancel an actively running Checkmarx scan
- **get_project**: Essential for ensuring the correct branch and source control context is selected before triggering new scans.

Get details for a specific Checkmarx project
- **get_kics_results**: Focuses solely on Terraform, CloudFormation, Kubernetes YAML, and Dockerfile misconfigurations rather than typical application source code flaws.

Get specialized Infrastructure as Code (KICS) findings
- **list_applications**: An Application acts as an overarching container for multiple individual microservices or projects, providing aggregated risk reporting and security metric visibility across a logical product.

List Checkmarx One Applications
- **list_bfl**: Provide the scan ID and the specific query (rule) ID string.

Get Best Fix Location (BFL) for a specific vulnerability node
- **list_projects**: A Project represents a specific codebase. Includes project metadata, IDs, and assigned application linkages.

List all Checkmarx One Projects
- **list_scans**: Includes the scan ID, current status (Completed, Running, Failed, Canceled), branch targeted, and timestamps. Use the scan ID to fetch the actual vulnerability results.

List all historical and active scans for a Checkmarx project
- **run_scan**: Extensively used in CI/CD integrations to assert security quality on PRs. Returns the ID of the newly queued scan.

Trigger a new Checkmarx One code scan
- **get_scan_details**: It returns granular execution details including which scan engines (SAST, SCA, KICS) were fired, their individual execution timings, and any engine-specific failure reasons.

Check the precise status and configuration of a Checkmarx scan
- **get_scan_results**: Each result includes the vulnerability severity, state (To Verify, Confirmed, Urgent), description, and the exact lines of code where the flaw was detected. Requires a completed scan ID.

Download SAST and security vulnerability findings for a scan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkmarx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most severe vulnerabilities found in the last Checkmarx scan."

**🤖 AI Agent:**
> Found 12 vulnerabilities in scan #4521. Critical: 2 SQL Injection (CWE-89) in `/api/users.js:142` and `/auth/login.ts:87`. High: 3 XSS (CWE-79). Medium: 7. Use `get_bfl` to find the optimal fix location for each.

---

**👤 You:**
> "Trigger a new SAST scan for my current Checkmarx project."

**🤖 AI Agent:**
> SAST scan initiated successfully for project 'web-app' on branch 'main'. Scan ID: #4522. Estimated completion: ~8 minutes. I'll notify you when results are ready.

---

**👤 You:**
> "How do I fix the SQL injection vulnerability found in the Checkmarx report?"

**🤖 AI Agent:**
> The SQL injection in `auth/login.ts:87` can be fixed by using parameterized queries. Best Fix Location (BFL) analysis shows the root cause is at line 82 where user input flows unsanitized into the query builder. Replace the string concatenation with a prepared statement.


## Installation & Usage

To install and use the **Checkmarx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkmarx](https://vinkius.com/mcp/checkmarx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
