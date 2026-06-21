# Tenable MCP Server

Manage Tenable Vulnerability Management scans, inspect cloud assets, and triage CVEs natively via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tenable)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect your **Tenable** (Tenable.io) environment to any AI agent and bring your enterprise vulnerability management directly into your IDE or chat via natural conversation.

### What you can do

- **Scans & Assessments** — List configured vulnerability scans, retrieve detailed run analytics, and even manually trigger immediate evaluations
- **Asset Intelligence** — Browse your entire host and cloud inventory, retrieving deep telemetry like OS fingerprints, IPs, and tags
- **Vulnerability Triage** — Pinpoint explicit security findings (Workbench) and CVEs affecting specific assets without navigating complex dashboards
- **Topology Oversight** — See how your network spaces overlap and track organizational logical folders
- **Scanner Health** — Check the operational status and plugin health of your internal enterprise scanning fleet

### How it works

1. Subscribe to this server
2. Enter your Tenable Access Key and Secret Key
3. Start investigating your risk exposure rapidly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts** — pull CVE details for a specific compromised server in a matter of seconds
- **DevSecOps Engineers** — manually trigger scans on newly deployed infrastructure zones right from their code editor
- **IT Administrators** — audit scanner health and check if host tags actually match the logical network topologies


## Available Tools
- **get_asset_details**: Retrieves detailed metadata, networking, and risk profile for a specific asset
- **get_asset_vulnerabilities**: Retrieves explicit security findings (Workbench) for a specific asset
- **get_scan_results**: Retrieves runtime analytics and vulnerability summaries for a specific scan
- **launch_scan**: Returns the newly created scan run ID.

Manually triggers an immediate execution of a configured scan
- **list_assets**: Lists host and cloud assets discovered in Tenable.io
- **list_scan_folders**: g. "My Scans", "PCI Quarters").

Lists operational scan folders
- **list_logical_networks**: Lists Tenable logical routing networks
- **list_scans**: Lists vulnerability assessment scans from Tenable.io
- **list_asset_tags**: g. "Critical", "Production", "External").

Lists organizational tags mapped to assets
- **list_scanners**: Lists Nessus scanners managed by Tenable.io


## Installation & Usage

To install and use the **Tenable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenable](https://vinkius.com/mcp/tenable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
