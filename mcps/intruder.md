# Intruder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/intruder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/intruder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/intruder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automate vulnerability scanning and security monitoring via Intruder.io API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intruder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active targets in my Intruder account."

**🤖 AI Agent:**
> I'll fetch the list of your infrastructure and application targets.

---

**👤 You:**
> "Show me the latest vulnerability issues found."

**🤖 AI Agent:**
> I'll retrieve the most recent security issues identified by Intruder.

---

**👤 You:**
> "Check the status of my recent scans."

**🤖 AI Agent:**
> I'll look up the history and current status of your vulnerability scans.


## Installation & Usage

To install and use the **Intruder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intruder](https://vinkius.com/mcp/intruder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
