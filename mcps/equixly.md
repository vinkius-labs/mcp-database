# Equixly MCP Server

Automate API security testing via Equixly — manage target services, trigger autonomous AI pentests, and audit vulnerability findings directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/equixly)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Equixly** account to any AI agent and take full control of your autonomous API security testing and vulnerability management through natural conversation.

### What you can do

- **Autonomous Pentest Orchestration** — Launch new attack sessions where the Equixly AI Hacker autonomously explores and attacks your API for BOLA, IDOR, and injection flaws
- **Service Management** — Register and manage target API services by defining base URLs and granular path-scoping rules for continuous monitoring
- **API Surface Discovery** — Upload and manage API specifications (OpenAPI, GraphQL, Postman) to broaden the attack surface known to the AI Hacker
- **Vulnerability Auditing** — Retrieve detailed lists of confirmed exploitable security flaws with severity ratings, OWASP mapping, and remediation guidance
- **Scan Status Monitoring** — Track execution progress and overall outcomes of active penetration tests, including total requests and endpoints explored
- **Remediation Oversight** — Access evidence of exploitation for specific findings to validate security fixes and maintain production safety
- **Target Configuration** — Fetch granular metadata for API targets, including authentication hooks and production safety toggles natively

### How it works

1. Subscribe to this server
2. Enter your Equixly API Token (found in your platform's Authentication Settings or Admin section)
3. Start managing your API security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers & CISOs** — monitor API security posture and trigger pentests without manual tool configuration
- **Backend Developers** — trigger security scans upon deployment and verify remediation guidance directly from the IDE
- **DevSecOps Teams** — integrate autonomous pentesting into CI/CD pipelines and audit findings using natural language
- **QA Engineers** — verify API security boundaries and test for business logic flaws through natural conversation


## Available Tools
- **create_service**: Provide the human-readable name and the live base URL. After creation, upload an API spec to maximize attack surface coverage.

Register a new API target service for autonomous pentesting
- **delete_service**: Use when decommissioning an API or cleaning up test environments. This action is irreversible.

Remove an API service and all its scan history from Equixly
- **get_scan_findings**: Each finding includes a severity rating, OWASP category, affected endpoint path, HTTP method, request/response evidence of exploitation, and actionable remediation guidance.

Download all exploitable vulnerabilities found in a pentest scan
- **get_scan**: Includes total requests made, endpoints explored, attack vectors attempted, severity breakdown of findings (critical/high/medium/low), and OWASP Top 10 mapping.

Get detailed status and summary of a specific pentest scan
- **get_service**: Required before modifying scan behavior.

Get detailed configuration of a specific API service
- **list_scans**: Each scan entry includes its status (running, completed, failed), timestamps, and the total count of vulnerabilities detected in that session.

List all pentest scan sessions for an API service
- **list_services**: A Service represents a single API base URL that the autonomous AI pentester continuously attacks. Each service contains its unique ID, name, base URL, and the number of discovered endpoints.

List all registered API services in Equixly
- **list_api_specs**: The AI Hacker uses these specs to understand the full attack surface, so keeping them updated maximizes vulnerability discovery coverage.

List uploaded API specifications for a service
- **trigger_scan**: It tests for BOLA, broken authentication, mass assignment, IDOR, injection, and business logic flaws. Ideal for CI/CD pipeline integration upon each deployment.

Launch a new autonomous AI penetration test against a service
- **upload_api_spec**: Supported formats: openapi (JSON/YAML), postman, graphql, wsdl, har. Pass the raw spec content as a string along with the format identifier.

Upload an API specification (OpenAPI, Postman, etc.) to a service


## Installation & Usage

To install and use the **Equixly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/equixly](https://vinkius.com/mcp/equixly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
