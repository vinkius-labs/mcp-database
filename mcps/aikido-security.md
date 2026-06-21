# Aikido Security MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aikido-security)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aikido-security-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aikido-security-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Query security vulnerabilities via Aikido — list open issues, check repositories, monitor cloud assets, and track compliance directly from any AI agent.

## Description
Connect your **Aikido Security** account to any AI agent and take full control of your security posture monitoring through natural conversation.

### What you can do

- **Open Issues** — List all open security vulnerabilities (CVEs, leaked secrets, cloud misconfigs, SAST findings) ordered by priority
- **Repository Scanning** — View all connected code repositories and their scanning status across GitHub, GitLab, Bitbucket
- **Cloud Asset Monitoring** — List cloud infrastructure assets from AWS, GCP, and Azure being monitored for misconfigurations
- **Container Security** — Monitor container images and registries for known vulnerabilities
- **Compliance Tracking** — Get ISO 27001 and SOC2 compliance overviews for audit preparation
- **Export Issues** — Bulk export all security findings for reporting and analysis
- **Webhook Management** — List configured webhooks for Slack, Jira, and other integrations

### How it works

1. Subscribe to this server
2. Enter your Aikido API token from User Settings > Personal Access Tokens
3. Start monitoring security issues, checking compliance, and auditing your posture from Claude, Cursor, or any MCP-compatible client

No more navigating the Aikido dashboard for every security review. Your AI acts as a dedicated security analyst.

### Who is this for?

- **Security Engineers** — instantly triage open vulnerabilities by severity and priority without opening the Aikido dashboard
- **DevOps Teams** — monitor cloud assets and container images for misconfigurations and known CVEs
- **Compliance Officers** — check ISO 27001 and SOC2 compliance status before audits
- **Engineering Managers** — export security reports and track remediation progress across teams


## Available Tools
- **export_all_issues**: This provides a comprehensive snapshot of your organization's security posture.
Use this for compliance reporting, audit preparation, or bulk analysis of vulnerabilities.

Export all security issues from Aikido
- **get_iso_compliance**: Shows which controls are passing, failing, or need attention.
Use this for compliance monitoring, audit preparation, and security posture reporting.
This endpoint is available on all paid Aikido plans.

Get ISO 27001 compliance overview for your organization
- **get_issue_group**: The issue group ID can be obtained from list_open_issues.
Each issue group represents a category of related vulnerabilities (e.g., the same CVE across multiple repositories).
Use this to deep-dive into a specific security finding before deciding on remediation steps.

Get detailed information about a specific security issue group
- **get_soc2_compliance**: Shows which trust service criteria are met and which need remediation.
Use this for SOC2 audit preparation and compliance monitoring.
This endpoint is available on all paid Aikido plans.

Get SOC2 compliance overview for your organization
- **get_workspace**: Use this to verify your workspace setup and check for any configuration errors.

Get workspace information and configuration
- **list_apps**: Shows which apps have active protection and their configuration status.
Use this to verify your web applications are properly secured against common attacks (SQL injection, XSS, etc.).

List all web applications protected by Aikido firewall
- **list_cloud_assets**: You can paginate through results and optionally search by text or sort by name, asset type, region, etc.
Use this to understand your cloud attack surface and identify misconfigurations or vulnerabilities.

List cloud infrastructure assets monitored by Aikido
- **list_code_repositories**: This includes repositories connected from GitHub, GitLab, Bitbucket, etc.
Use this to discover which repositories are being monitored for vulnerabilities and security issues.

List all active code repositories connected to Aikido
- **list_connected_clouds**: Shows which cloud environments are being monitored for security misconfigurations and vulnerabilities.
Use this to verify cloud integrations are properly configured.

List all cloud accounts connected to Aikido
- **list_containers**: This includes Docker images from registries like Docker Hub, ECR, GCR, etc.
Use this to monitor container security and identify vulnerable base images or dependencies.

List all container images and repositories scanned by Aikido
- **list_custom_rules**: Custom rules allow you to define organization-specific security checks beyond the default scanner.
Use this to audit your custom rule coverage and ensure your security policies are properly enforced.

List all custom SAST scanning rules in Aikido
- **list_open_issues**: Issues include vulnerabilities from code scanning, container scanning, cloud security, SAST, IaC, DAST, and more.
You can optionally filter by issue type (open_source, leaked_secret, cloud, sast, iac, docker_container, etc.),
by team ID, or by repository. Supports pagination with page and per_page parameters.
Use this to get a comprehensive view of your organization's security posture and prioritize remediation efforts.

List all open security issues (vulnerabilities) in your Aikido account
- **list_teams**: Teams are used to organize repositories, assign issues, and manage security workflows.
Use this to understand how your organization structures its security responsibilities.

List all teams in your Aikido organization
- **list_users**: Shows user roles, permissions, and access levels.
Use this to audit user access and ensure proper security team membership.

List all users in your Aikido organization
- **list_virtual_machines**: Use this to understand your VM attack surface and identify security gaps.

List all virtual machines monitored by Aikido
- **list_webhooks**: Webhooks are used to send security event notifications to external systems (Slack, Jira, etc.).
Use this to verify integrations are properly configured and troubleshoot notification delivery.

List all configured webhooks in Aikido


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aikido Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all critical and high severity open security issues, grouped by type."

**🤖 AI Agent:**
> I've retrieved your open issues. You currently have 23 open issue groups: 4 CRITICAL (including 2 actively exploited CVEs in log4j), 12 HIGH (mostly outdated dependencies and exposed secrets), 5 MEDIUM, and 2 LOW. Top priority: CVE-2024-1234 affecting 3 repositories — patch available. Would you like the full details of any specific issue group?

---

**👤 You:**
> "What's our current ISO 27001 compliance status?"

**🤖 AI Agent:**
> Your ISO 27001 compliance overview shows 89% of controls passing (142/160). Areas needing attention: A.8.25 (Secure Development Lifecycle) — 3 failing checks, A.8.28 (Secure Coding) — 2 failing checks. All other control categories are passing. You're well-positioned for your next audit. Would you like the full breakdown by control category?

---

**👤 You:**
> "List all our connected cloud accounts and any misconfigurations found in the last 7 days."

**🤖 AI Agent:**
> You have 3 connected cloud accounts: AWS (production), GCP (staging), Azure (dev). In the last 7 days, Aikido found 5 new cloud misconfigurations: 2 public S3 buckets in production AWS, 1 over-permissive IAM role in GCP, and 2 unencrypted RDS instances in AWS staging. All are classified as HIGH priority. Would you like the details of any specific misconfiguration?


## Installation & Usage

To install and use the **Aikido Security** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aikido-security](https://vinkius.com/mcp/aikido-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
