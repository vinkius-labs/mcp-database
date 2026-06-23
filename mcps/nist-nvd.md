# NIST NVD MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nist-nvd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access authoritative vulnerability and product data via NIST NVD — track CVEs, CPEs, and security history directly from your AI agent.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NIST NVD** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the details for CVE-2023-23397."

**🤖 AI Agent:**
> Retrieving CVE-2023-23397... This is a Critical elevation of privilege vulnerability in Microsoft Outlook with a CVSS score of 9.8. It allows an attacker to steal NTLM hashes. Would you like to see the list of affected software versions (CPEs)?

---

**👤 You:**
> "Search for vulnerabilities in 'WordPress' with CRITICAL severity."

**🤖 AI Agent:**
> Searching NVD... I've found several critical vulnerabilities affecting WordPress core and popular plugins. The most recent include CVE-2023-XXXX (Remote Code Execution). Shall I provide the full description for the most recent one?

---

**👤 You:**
> "What is the official CPE name for 'Windows 11'?"

**🤖 AI Agent:**
> Querying CPE dictionary... The primary CPE 2.3 name for Windows 11 is 'cpe:2.3:o:microsoft:windows_11:-:*:*:*:*:*:*:*'. I also found specific versions for various builds. Would you like to search for CVEs affecting this specific CPE?


## ❓ FAQ

**Q: Is an API Key mandatory?**
No. The NVD API allows public access without a key. However, using a key increases your rate limit significantly (up to 50 requests per 30 seconds).

**Q: What is a CPE string?**
CPE (Common Platform Enumeration) is a structured naming scheme for information technology systems, software, and packages (e.g., cpe:2.3:a:microsoft:exchange_server:2019).

**Q: How far back can I search for vulnerabilities?**
The NVD contains vulnerabilities dating back to the late 1990s. You can search the entire database by ID or keyword.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nist-nvd](https://vinkius.com/mcp/nist-nvd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NIST NVD** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nist-nvd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NIST NVD** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nist-nvd": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
