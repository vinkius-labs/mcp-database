# AbuseIPDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abuseipdb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/abuseipdb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/abuseipdb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Audit IP addresses — check abuse scores and reports via AI.

## Description
Empower your AI agent to orchestrate your entire network security and IP auditing workflow with **AbuseIPDB**, the leading source for crowdsourced IP reputation data. By connecting the AbuseIPDB API to your agent, you transform complex security lookups into a natural conversation. Your agent can instantly check IP addresses for malicious activity, audit abuse confidence scores, and retrieve detailed reporting history without you ever touching a security dashboard. Whether you are conducting forensic analysis or monitoring server logs, your agent acts as a real-time security consultant, ensuring your network data is always verified and precise.

### What you can do

- **IP Auditing** — Check any IPv4 or IPv6 address against the global abuse database and retrieve high-resolution reputation metadata.
- **Confidence Oversight** — Audit the abuse confidence score for specific IPs to understand the likelihood of malicious intent instantly.
- **Report Discovery** — Retrieve detailed reporting history for an IP address to identify patterns of spam, hacking, or DDoS activity.
- **Blacklist Intelligence** — Query the current global blacklist of most reported IPs to maintain strict organizational control over network access.
- **Operational Monitoring** — Check API status to ensure your security research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your AbuseIPDB API Key
3. Start managing your network intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts & CISOs** — monitor IP reputations and retrieve official metadata straight from your workflow.
- **DevOps Engineers** — verify server logs and audit incoming traffic patterns without manual searching.
- **Network Administrators** — perform rapid audits of suspicious IPs and identify relevant security markers through natural language.
- **Operations Leads** — automate security data querying to orchestrate cross-functional infrastructure teams smoothly.


## Available Tools
- **check_ip_address**: Check an IP address against the AbuseIPDB database
- **check_api_status**: Check if the AbuseIPDB service is operational
- **get_abuse_blacklist**: Retrieve the current list of most reported IP addresses
- **get_ip_abuse_reports**: Get a list of reports for a specific IP address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AbuseIPDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check IP address '1.2.3.4' using AbuseIPDB."

**🤖 AI Agent:**
> I've retrieved the reputation data for 1.2.3.4! The Abuse Confidence Score is currently 85%, which is identified as 'High Risk'. It has been reported over 50 times recently. Would you like the detailed report history?

---

**👤 You:**
> "Show recent abuse reports for IP '192.168.1.1'."

**🤖 AI Agent:**
> I've identified the reports for 192.168.1.1. No reports were found in the last 90 days, resulting in a confidence score of 0%. I can assist you with a deep-dive lookup if you suspect hidden activity.

---

**👤 You:**
> "Get the current blacklist of top 100 reported IPs."

**🤖 AI Agent:**
> I've retrieved the current global blacklist! Notable entries include IPs associated with recent massive brute-force attacks. I can provide the abuse scores and country metadata for each of these addresses.


## Installation & Usage

To install and use the **AbuseIPDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abuseipdb](https://vinkius.com/mcp/abuseipdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
