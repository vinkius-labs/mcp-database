# Socket.dev (Dependency Security) MCP Server

Protect your software supply chain by scanning dependencies, checking package security scores, and monitoring threat feeds directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/socketdev-dependency-security)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect **Socket.dev** to your AI agent to proactively defend against supply chain attacks. This MCP server allows you to analyze open-source packages, scan manifest files, and monitor for malicious dependencies without leaving your development environment.

### What you can do

- **Package Analysis** — Get deep security scores and identify issues for specific packages using PURLs (e.g., npm, PyPI, Go).
- **Dependency Scanning** — Upload manifest files like `package.json` or `requirements.txt` to create comprehensive security scans.
- **Report Management** — List and retrieve detailed security reports, including policy compliance and alert data.
- **Threat Intelligence** — Access a real-time feed of malicious packages detected by Socket's analysis engine.
- **Organization Oversight** — Manage scans across different organizations and monitor your API usage quotas.

### How it works

1. Subscribe to this server
2. Enter your Socket.dev API Token
3. Start auditing your dependencies directly from Claude, Cursor, or any MCP-compatible client

Stop guessing if a package is safe. Let your AI agent use Socket's industry-leading telemetry to catch typosquatting, backdoors, and telemetry before they enter your codebase.

### Who is this for?

- **Security Engineers** — Automate the review of new dependencies and monitor organizational security posture.
- **Developers** — Check package safety scores instantly before running `npm install` or `pip install`.
- **DevOps Teams** — Integrate dependency scanning into the conversation to quickly triage security reports.


## Available Tools
- **create_scan**: Provide manifest files data (e.g., package.json, requirements.txt).

Create a new scan by uploading manifest files
- **delete_scan**: Delete a scan
- **get_package_issues**: g., pkg:npm/babel).

Get issues/alerts for a specific package
- **get_package_score**: g., pkg:npm/babel).

Get the security score for a specific package
- **get_quota**: Check remaining API quota
- **get_report**: Get detailed report data
- **get_scan**: Get scan metadata and status
- **get_threat_feed**: Access the real-time threat feed
- **list_organizations**: List organizations the token has access to
- **list_reports**: List reports


## Installation & Usage

To install and use the **Socket.dev (Dependency Security)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/socketdev-dependency-security](https://vinkius.com/mcp/socketdev-dependency-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
