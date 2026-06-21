# Aikido Security MCP Server

Query security vulnerabilities via Aikido — list open issues, check repositories, monitor cloud assets, and track compliance directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aikido-security)

## Overview
**Category:** fort-knox
**Tools Count:** 16

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


## Installation & Usage

To install and use the **Aikido Security** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aikido-security](https://vinkius.com/mcp/aikido-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
