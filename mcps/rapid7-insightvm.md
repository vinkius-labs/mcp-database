# Rapid7 InsightVM MCP Server

Equip your AI to interact directly with Rapid7 InsightVM, extracting vulnerability assessments, scanning network assets, and launching immediate scans.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rapid7-insightvm)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect your **Rapid7 InsightVM** (formerly Nexpose) platform directly to your AI agent. By granting this access, your AI becomes a highly interactive cybersecurity assistant, allowing engineers and security analysts to query vulnerabilities, review asset health, and start scans right from their workspace or IDE.

### What you can do

- **Asset Querying** — Retrieve comprehensive inventory lists to discover all tracked computing assets and read their operating system fingerprints and hardware information.
- **Vulnerability Checks** — Scan specific assets to instantly read CVE numbers mapped against them, alongside full vulnerability advisories and remediation guidelines.
- **Scan Operations** — Read chronologically maintained assessment scans and track their execution status without jumping between consoles.
- **Site Management** — Explore configured network sites, observing their designated scanning scopes and reviewing overall health risks.
- **Trigger Scanning** — Force an immediate re-evaluation scan on a specified site after applying a patch, validating your resolution securely.

### How it works

1. Authorize the server module inside your environment.
2. Add the URL and port of your Rapid7 Security Console alongside a dedicated set of credentials (username and password) configured as Basic Authentication.
3. Chat with your AI to start asking about the latest threats affecting your domain servers.

### Who is this for?

- **Cybersecurity Analysts (SOC)** — Analyze identified security flaws and fetch CVE details and remediation instructions without leaving their incident response platform.
- **DevOps & SysAdmins** — Quickly order a vulnerability assessment on a subnet after applying OS updates to check if the threat is successfully patched.
- **Network Engineers** — Evaluate site configurations directly when provisioning new subnets to ensure full scanning scope coverage.


## Available Tools
- **get_asset**: Retrieves detailed information for a specific asset
- **get_asset_vulnerabilities**: Lists all vulnerabilities found on a specific asset
- **get_scan**: Retrieves execution status and results for a specific scan
- **get_site**: Retrieves details for a specific network site
- **get_vulnerability**: Retrieves details for a specific vulnerability ID
- **list_assets**: Lists all discovered computing assets
- **list_scans**: Lists chronological assessment scans
- **list_sites**: Lists all configured network scan sites
- **list_vulnerabilities**: Lists global vulnerability definitions
- **trigger_scan**: Forces an immediate vulnerability scan for a site


## Installation & Usage

To install and use the **Rapid7 InsightVM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rapid7-insightvm](https://vinkius.com/mcp/rapid7-insightvm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
