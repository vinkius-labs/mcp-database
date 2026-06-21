# Wallarm MCP Server

Monitor API security, detect attacks, and manage WAF vulnerabilities on Wallarm — the end-to-end API security platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wallarm)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect your **Wallarm** account to any AI agent and secure your API infrastructure through natural conversation.

### What you can do

- **Security Attacks** — Monitor and search for active security attacks detected by Wallarm, grouped by vector (SQLi, XSS, etc.)
- **Granular Hits** — Perform deep forensics by searching for individual malicious HTTP request hits with full payloads
- **Vulnerability Management** — List and triage security vulnerabilities discovered in live API traffic directly from your agent
- **API Inventory** — Retrieve the automatically discovered API inventory to see all exposed endpoints and methods
- **Filtering Nodes** — Verify the health and heartbeat status of your deployed WAF and API gateway filtering nodes
- **IP Control** — Audit and manage IP allowlist/denylist rules to immediately block malicious sources or allow trusted partners
- **Remediation Guidance** — Access comprehensive diagnostic data and CWE mappings for specific vulnerabilities

### How it works

1. Subscribe to this server
2. Enter your Wallarm API Token and Client ID
3. Start monitoring your API security posture through Claude, Cursor, or any MCP-compatible client

No more manual digging through security consoles to find attack patterns. Your AI agent becomes your SOC security analyst.

### Who is this for?

- **Security Engineers (DevSecOps)** — monitor live threats and triage vulnerabilities during the development lifecycle
- **SOC Analysts** — perform rapid incident forensics and block malicious IPs through simple chat commands
- **API Developers** — discover exposed endpoints and verify the security posture of internal and external APIs
- **SRE & Platform Teams** — monitor the health of security edge nodes and manage global access rules efficiently


## Available Tools
- **create_ip_acl_rule**: list_type must be "white" or "black".

Adds an IP or CIDR range to the global allowlist or denylist
- **get_discovered_api_inventory**: Retrieves the API inventory automatically discovered through passive traffic analysis
- **get_client_info**: Retrieves details about the Wallarm account, subscription, and feature status
- **get_vulnerability_details**: Retrieves comprehensive diagnostic data and exploit evidence for a specific vulnerability ID
- **list_ip_acl_rules**: Lists configured IP allowlist and denylist rules
- **list_filtering_nodes**: Lists all deployed Wallarm WAF/API gateway filtering nodes
- **search_security_attacks**: Searches for security attacks detected by Wallarm, grouped by vector (SQLi, XSS, etc.)
- **search_security_hits**: Shows full request headers and payloads for blocked traffic.

Searches for granular individual malicious HTTP request hits intercepted by WAF nodes
- **search_vulnerabilities**: Lists all open security vulnerabilities discovered in live API traffic
- **update_vulnerability_status**: Valid statuses: open, closed, falsepositive.

Changes the lifecycle status of a vulnerability (e.g., mark as closed or false positive)


## Installation & Usage

To install and use the **Wallarm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wallarm](https://vinkius.com/mcp/wallarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
