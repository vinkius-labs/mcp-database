# Veracode MCP Server

Bring Veracode AppSec to your AI. Analyze source code flaws, extract application profiles, and track vulnerabilities conversationaly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/veracode)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Equip your AI agent with complete read and write access to your **Veracode** ecosystem. Seamlessly blend application security posture management alongside your typical development workflow using entirely conversational AI.

### What you can do

- **Unified Vulnerability Tracing** — Ask the agent to list Open security findings or mitigation statuses spanning across Static (SAST), Dynamic (DAST), and Component (SCA) analytics per application.
- **Deep Flaw Details** — Input specific Finding IDs and let the bot explain the underlying CWE error, affected code strings, severity ratings, and automated remediation tutorials.
- **Portfolio AppSec Management** — List tracked applications, create novel application profiles on the fly before a commit, or request health checks mapping sandbox testing environments.
- **Dynamic Scan Queries** — Poll your AI intuitively ensuring it retrieves the real-time execution bounds of your scheduled Web Application Security runtime scenarios.

### How it works

1. Subscribe to this connected server
2. Securely provide your dual Veracode API ID and API Secret pair
3. Engage directly with Claude, Cursor, or compatible clients querying security intelligence intuitively

### Who is this for?

- **DevSecOps Engineers** — bypass extensive console clicking to check scan statuses and manually export flaws by chatting internally for a summary.
- **Application Developers** — fix security defects natively in Cursor by commanding it to read the flawed line out of the Veracode finding ID report directly.
- **CISO & Security Managers** — audit all authenticated identity users or track general application risk matrices effortlessly reading human-summarized text outputs.


## Available Tools
- **create_application**: Provide the app schema and profile name as a JSON string.

Create a new Veracode application profile container
- **delete_application**: This action is irreversible.

Delete a Veracode application permanently
- **get_api_health**: Check the health of Veracode connection
- **get_application_details**: Information includes its Veracode compliance policy status, business criticality rating, deployment state, and risk scores.

Get a detailed profile of a Veracode application
- **get_finding_details**: Explains the vulnerability type (CWE), affected source file, code path, and remediation guidance.

Get precise vulnerability details for a specific flaw/finding
- **list_applications**: Most structural entities return a globally unique GUID which is required for sub-resource lookups.

List all Veracode AppSec Applications
- **list_dynamic_analyses**: List configured Dynamic Analysis (DAST) scans
- **list_security_findings**: Retrieve the unified security findings for an application
- **list_sandboxes**: List all testing sandboxes linked to an application
- **list_veracode_users**: Used to manage RBAC roles.

List authorized Veracode identity users


## Installation & Usage

To install and use the **Veracode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veracode](https://vinkius.com/mcp/veracode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
