# Rapid7 InsightVM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rapid7-insightvm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Equip your AI to interact directly with Rapid7 InsightVM, extracting vulnerability assessments, scanning network assets, and launching immediate scans.

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


## Available Tools (10)
- **get_site**: Retrieves details for a specific network site
- **get_vulnerability**: Retrieves details for a specific vulnerability ID
- **list_assets**: Lists all discovered computing assets
- **list_scans**: Lists chronological assessment scans
- **list_sites**: Lists all configured network scan sites
- **list_vulnerabilities**: Lists global vulnerability definitions
- **trigger_scan**: Forces an immediate vulnerability scan for a site
- **get_asset**: Retrieves detailed information for a specific asset
- **get_asset_vulnerabilities**: Lists all vulnerabilities found on a specific asset
- **get_scan**: Retrieves execution status and results for a specific scan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rapid7 InsightVM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the list of network sites currently managed by Rapid7."

**🤖 AI Agent:**
> Using the `list_sites` command, I found 3 network targets: 'London Head Office' (ID: 10), 'Cloud AWS Infrastructure' (ID: 12), and 'Guest WiFi Segment' (ID: 15).

---

**👤 You:**
> "What vulnerabilities are discovered on asset 1052?"

**🤖 AI Agent:**
> I queried `get_asset_vulnerabilities` for asset 1052. The host has 5 active vulnerabilities, primarily unpatched OpenSSL packages triggering high-severity CVE-2023-XXXX listings.

---

**👤 You:**
> "Force a new scan on Site ID 15 immediately."

**🤖 AI Agent:**
> I submitted the `trigger_scan` command for Site ID 15. The InsightVM engine has confirmed the execution, and the scan is now running in the background. You can check its progress shortly using queries.


## ❓ FAQ

**Q: How do I configure my credentials for Rapid7?**
The integration uses Basic Authentication interacting with the Rapid7 Console API. You must configure the `RAPID7_HOST` (IP or FQDN), `RAPID7_PORT` (usually 3780), along with a dedicated `RAPID7_USER` and `RAPID7_PASSWORD`. We strongly recommend generating a specific service account in your console with restricted scan permissions.

**Q: Is the scanning triggered individually per asset?**
By default, the `trigger_scan` mechanism relies on referencing a defined `site_id`, scanning the preconfigured scope attached to it rather than blindly scanning one unassociated IP.

**Q: Does it report CVSS scores?**
Yes, depending on the response data provided by your installed version of the InsightVM console. Using `get_vulnerability` or checking asset lists brings standard threat metadata and corresponding CVSS vectors directly into your AI interface context.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rapid7-insightvm](https://vinkius.com/mcp/rapid7-insightvm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rapid7 InsightVM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rapid7-insightvm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rapid7 InsightVM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rapid7-insightvm": {
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
