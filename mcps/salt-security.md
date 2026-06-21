# Salt Security MCP Server

Integrate Salt Security directly with your AI for comprehensive API threat vector discovery, posture management, and active remediation in real-time.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salt-security)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect your AI directly with **Salt Security** to proactively defend your Application Programming Interface (API) environment. Improve API discovery, manage security posture, and remediate threats in real-time through simple conversational prompts.

### What you can do

- **API Inventory & Discovery** — View all auto-discovered APIs in your environment, including unknown or shadow APIs (`get_inventory`). Retrieve schema details, identify exposed sensitive data (PII), and analyze structural drifts (`get_endpoint`).
- **Threat Intelligence & Monitoring** — Monitor active API attacks and business logic abuses as they happen (`get_attacks`). Profile known threat actors to uncover behavioral patterns (`get_attackers`).
- **Active Remediation** — Respond to incidents immediately by triggering blockade commands against attackers, seamlessly passing instructions to your integrated WAFs (`block_attacker`).
- **Posture & Governance Assessment** — Identify design flaws and vulnerabilities before they reach production (`get_posture_vulnerabilities`). Manage OpenAPI (OAS) specifications (`list_oas_specs`, `upload_oas_spec`) and verify active governance rules (`get_governance_policies`).

### How it works

1. Enable the Salt Security integration in your workspace.
2. Navigate to your Salt Security console.
3. Go to the Settings or Administration section and generate a new API Token.
4. Paste this token securely into the configuration fields provided below.
5. Ask the AI: "Are there any known threat actors exploiting our APIs right now?"


## Available Tools
- **block_attacker**: Issues a command to block a specific attacker
- **get_attackers**: Lists known threat actors profiled by Salt
- **get_attacks**: Lists detected malicious API attacks
- **get_endpoint**: Retrieves details for a specific API endpoint
- **get_governance_policies**: Lists active API governance rules
- **get_inventory**: Retrieves the auto-discovered API inventory
- **get_posture_vulnerabilities**: Retrieves identified pre-production design flaws
- **get_system_health**: Checks the health of traffic mirror ingestion
- **list_oas_specs**: Lists all uploaded OpenAPI specifications
- **upload_oas_spec**: Uploads a new OAS/Swagger specification


## Installation & Usage

To install and use the **Salt Security** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salt-security](https://vinkius.com/mcp/salt-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
