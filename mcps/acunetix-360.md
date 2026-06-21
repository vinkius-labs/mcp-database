# Acunetix 360 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acunetix-360)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/acunetix-360-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/acunetix-360-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automated web vulnerability scanning — manage scans, track issues, and audit security via AI.

## Description
Connect your **Acunetix 360** account to your AI agent to automate your web application security workflow. From launching new vulnerability scans to auditing identified security issues across your infrastructure, your agent manages application security through natural conversation.

### What you can do

- **Automated Scanning** — Launch new vulnerability scans for your web applications and APIs directly from chat
- **Issue Tracking** — List and retrieve detailed information on identified vulnerabilities, including severity levels and remediation tips
- **Scan Monitoring** — Track the progress and status of active security scans across your organization
- **Security Auditing** — Quickly retrieve a list of all identified issues to support compliance and risk management
- **CI/CD Integration Support** — Audit scan results from recent builds to ensure security is maintained throughout the development lifecycle

### How it works

1. Subscribe to this server
2. Enter your Acunetix 360 User ID and API Token
3. Start monitoring and managing your application security through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate vulnerability triage and monitor large-scale scanning operations
- **DevSecOps Teams** — integrate automated security checks intoCI/CD pipelines and audit results via AI
- **Web Developers** — quickly check for vulnerabilities in their applications during the development phase
- **Compliance Officers** — retrieve security reports and audit logs for risk assessment


## Available Tools
- **list_scans**: List vulnerability scans
- **launch_scan**: Start a new security scan
- **list_vulnerabilities**: List all identified security issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acunetix 360** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all high-severity vulnerabilities found in my last scan."

**🤖 AI Agent:**
> I've retrieved the identified issues. Your last scan found 3 high-severity vulnerabilities, including a SQL Injection and two Cross-Site Scripting (XSS) flaws. Would you like the remediation details for these?


## Installation & Usage

To install and use the **Acunetix 360** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acunetix-360](https://vinkius.com/mcp/acunetix-360)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
