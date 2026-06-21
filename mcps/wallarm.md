# Wallarm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wallarm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wallarm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wallarm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Monitor API security, detect attacks, and manage WAF vulnerabilities on Wallarm — the end-to-end API security platform.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wallarm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all security attacks detected in the last hour."

**🤖 AI Agent:**
> I've searched the recent security events in Wallarm. I found 12 attacks clusters, including 3 SQL Injections targeting the /api/login endpoint and 5 XSS attempts on /search. Would you like to see the individual hits and payloads for any of these?

---

**👤 You:**
> "Block the malicious IP address 1.2.3.4 immediately."

**🤖 AI Agent:**
> Understood. I have successfully added 1.2.3.4 to your global denylist (black list) in Wallarm. All traffic from this IP will now be blocked by your filtering nodes. Would you like to see if there are other IPs with similar behavior?

---

**👤 You:**
> "What vulnerabilities are currently open in our production API?"

**🤖 AI Agent:**
> I found 3 open vulnerabilities: 1. Broken Object Level Authorization (BOLA) on /api/user/{id} (Critical), 2. Information Disclosure via verbose error messages (Medium), and 3. Insecure Direct Object Reference (IDOR) on /api/orders (High). I can provide the remediation guidance for any of these.


## Installation & Usage

To install and use the **Wallarm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wallarm](https://vinkius.com/mcp/wallarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
