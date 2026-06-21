# Intruder MCP Server

Automate vulnerability scanning and security monitoring via Intruder.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/intruder)

## Overview
**Category:** security-compliance
**Tools Count:** 10

## Description
Empower your AI agents to manage your cybersecurity posture with Intruder.io. This MCP server allows you to list security targets, track vulnerability scans, retrieve identified issues, and monitor cloud integrations directly through the Intruder API. Ideal for automating DevSecOps workflows and security auditing.


## Available Tools
- **get_account**: Use to verify identity and account settings.

Gets your Intruder account details
- **get_issue**: Returns detailed descriptions, remediation advice, and affected targets. Essential for investigating and fixing security flaws.

Retrieves details for a specific issue
- **get_scan**: Returns the list of targets included, scan duration, and a summary of findings. Use this to audit the results of a specific security assessment.

Retrieves details for a specific scan
- **get_target**: Returns metadata and associated tags. Use this to deep-dive into the security status of a specific asset.

Retrieves details for a specific target
- **list_cloud_integrations**: Essential for auditing how Intruder discovers new targets in the cloud infrastructure.

Lists all configured cloud integrations (AWS, Azure, Google Cloud)
- **list_issues**: Returns issue titles, severity levels (Low, Medium, High, Critical), and status. Use this as the primary tool for security posture auditing.

Lists all identified vulnerability issues
- **list_licences**: Useful for verifying subscription status and capacity.

Lists all account licences
- **list_scans**: Includes scan types, timestamps, and IDs. Essential for tracking scan frequency and monitoring ongoing security checks.

Lists all vulnerability scans
- **list_targets**: Returns target names, IDs, and types. Use this to identify which assets are being scanned for vulnerabilities.

Lists all infrastructure and application targets
- **list_teams**: Useful for understanding organizational access controls.

Lists all organization teams


## Installation & Usage

To install and use the **Intruder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intruder](https://vinkius.com/mcp/intruder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
