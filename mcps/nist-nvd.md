# NIST NVD MCP Server

Access authoritative vulnerability and product data via NIST NVD — track CVEs, CPEs, and security history directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nist-nvd)

## Overview
**Category:** the-unthinkable
**Tools Count:** 10

## Description
Connect to the **National Vulnerability Database (NVD)** API through your AI agent and explore the world's most comprehensive archive of cybersecurity vulnerabilities and product data using natural conversation.

### What you can do

- **CVE Discovery** — Search for Common Vulnerabilities and Exposures (CVEs) by ID, keyword, or specific weakness (CWE).
- **Product Security** — Find all vulnerabilities associated with a specific product or version using its Common Platform Enumeration (CPE) string.
- **Severity Analysis** — Filter vulnerabilities based on their CVSS V3 severity level (Low to Critical) to prioritize risks.
- **Temporal Tracking** — Search for CVEs published or modified within specific date ranges to monitor recent threats.
- **Product Dictionary** — Query the official CPE dictionary by keyword or UUID to identify software and hardware products.
- **Change History** — Retrieve a detailed log of updates and modifications made to the vulnerability database.

### How it works

1. Subscribe to this server
2. (Optional) Enter your NIST NVD API Key for higher rate limits
3. Start exploring vulnerability intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Researchers & Analysts** — quickly retrieve CVE details or CVSS scores for risk assessment and mitigation.
- **DevOps & IT Teams** — monitor for new vulnerabilities affecting the specific products and versions in your stack.
- **Compliance Officers** — automate the gathering of vulnerability data for security audits and reporting.


## Available Tools
- **get_cpe_by_id**: Get CPE dictionary entry by UUID
- **get_cve_by_id**: g. CVE-2023-1234).

Get CVE details by ID
- **get_cve_change_history**: Retrieve CVE change history
- **list_cpe_matches**: List valid CPE match strings
- **search_cpe_by_keyword**: Search product dictionary by keyword
- **search_cve_by_cpe**: Find CVEs for a product (CPE)
- **search_cve_by_cwe**: g. CWE-89).

Find CVEs by weakness (CWE)
- **search_cve_by_date**: Search CVEs by publication date
- **search_cve_by_keyword**: Search CVEs by keyword
- **search_cve_by_severity**: Filter CVEs by severity


## Installation & Usage

To install and use the **NIST NVD** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nist-nvd](https://vinkius.com/mcp/nist-nvd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
