# FOSSA (License Compliance) MCP Server

Manage license compliance and security vulnerabilities via FOSSA — list projects, inspect revisions, and track dependencies directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fossa-license-compliance)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect your **FOSSA** account to any AI agent to automate open-source license compliance and security auditing through natural language.

### What you can do

- **Project Overview** — List all projects in your organization with support for filtering and pagination.
- **Revision Tracking** — Access specific project revisions and fetch detailed metadata for any version locator.
- **Dependency Analysis** — Deep-dive into the dependency tree of any revision to understand your software bill of materials (SBOM).
- **Impact Assessment** — Identify every parent project that contains a specific vulnerable or non-compliant dependency.
- **Vulnerability Scanning** — Check for security vulnerabilities across multiple dependency locators in a single query.

### How it works

1. Subscribe to this server
2. Enter your FOSSA API Token
3. Start auditing your software supply chain from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Engineers** — quickly identify where vulnerable packages are used across the entire organization.
- **Legal & Compliance Teams** — audit project revisions for license compliance without manually navigating the FOSSA UI.
- **DevOps & Architects** — verify dependency trees and project metadata directly from the terminal or code editor.


## Available Tools
- **check_vulnerabilities**: Uses a POST request but only reads data.

Check vulnerabilities by dependency locators
- **get_revision**: Get details for a specific revision
- **get_parent_projects**: Get parent projects containing a dependency
- **list_projects**: Supports filtering and pagination.

List all projects in your organization
- **get_revision_dependencies**: Get dependencies for a specific revision
- **list_revisions**: List revisions of a project


## Installation & Usage

To install and use the **FOSSA (License Compliance)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fossa-license-compliance](https://vinkius.com/mcp/fossa-license-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
