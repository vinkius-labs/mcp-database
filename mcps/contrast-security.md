# Contrast Security MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contrast-security)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Equip your AI with Contrast Security AppSec data to monitor applications and hunt critical vulnerabilities directly via chat.

## Description
Connect your **Contrast Security** platform to any AI agent and bring powerful AppSec monitoring to your conversational workflow. Instantly audit the security posture of your applications without digging through complex UI menus.

### What you can do

- **Application Triage** — Quickly list all monitored applications to ensure your Contrast sensors are actively covering your production and staging environments.
- **Vulnerability Hunting** — Query the AI to extract critical vulnerabilities (traces) across your entire app portfolio instantly, pulling precise flaws to prioritize remediation.
- **Trace Analysis** — Zoom in on a specific trace UUID to understand the security context and the exact affected endpoint.

### How it works

1. Subscribe to this security server
2. Authorize it using your Contrast Application API keys and Org ID
3. Start querying vulnerability traces from Claude, Cursor, or your MCP client

### Who is this for?

- **Security Engineers (SecOps)** — Query live vulnerability data from chat while actively writing triage tickets.
- **Developers** — Retrieve the specific details of a flagged vulnerability directly inside Cursor or VS Code without opening external platforms.
- **DevOps Leads** — Audit the operational status of Contrast sensors across fleet applications automatically through the AI.


## Available Tools (10)
- **get_application_details**: Get detailed information about a specific application
- **get_organization_info**: Get metadata about the current Contrast organization
- **get_vulnerability_details**: Get full technical details for a specific vulnerability trace
- **list_applications**: List all applications monitored in Contrast Security
- **list_critical_vulnerabilities**: Quickly list only vulnerabilities with CRITICAL severity
- **list_monitored_servers**: List servers where Contrast agents are deployed
- **list_vulnerability_traces**: List security vulnerability traces (vulnerabilities)
- **list_organization_users**: List users in your Contrast Security organization
- **search_applications_by_name**: Search for monitored applications by name
- **search_vulnerabilities**: Search and filter vulnerabilities using complex criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contrast Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications monitored in my Contrast Security organization."

**🤖 AI Agent:**
> I've fetched 3 active applications monitored under your umbrella: `Frontend-API`, `Backend-Payment-Engine`, and `Legacy-Staging-App`. Would you like to dig into the security score of a specific one?

---

**👤 You:**
> "List all CRITICAL vulnerabilities found across my entire Contrast fleet."

**🤖 AI Agent:**
> I found 2 traces classified as CRITICAL priority. 1) SQL Injection mapping to UUID `1xx-bbxx-11x` on application 'Backend-API'. 2) Deserialization exploit UUID `4yxx-bbx-22` on 'Legacy-Staging-App'.

---

**👤 You:**
> "Retrieve the full technical details for the vulnerability trace UUID '1xx-bbxx-11x'."

**🤖 AI Agent:**
> Decompressing trace `1xx-bbxx-11x`... It's flagged as an untrusted SQL Injection caused by vulnerable code in controller `AuthRoute.js` line 45. The status is open and currently untriaged.


## ❓ FAQ

**Q: How do I find my Contrast Security API credentials?**
Log into your Contrast Security web interface. Navigate directly to your profile dropdown via **User Settings** -> **Profile**. Here you will find your distinct Authorization Key (encoded string), API Key, and the required Organization UUID at the very top.

**Q: What exactly is termed a 'Trace' in the Contrast ecosystem?**
A Trace is the Contrast terminology applied to a single explicit instance of a security vulnerability uncovered deep within an executing application. Every trace holds a massive amount of payload data concerning the attack vectors.

**Q: Can I use this MCP integration to completely delete trace incidents?**
No. The integration architecture focuses heavily on purely read-only auditing workflows. Features like permanently overwriting and deleting incident historical data are prohibited to ensure strong forensic compliance logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contrast-security](https://vinkius.com/mcp/contrast-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contrast Security** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contrast-security` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contrast Security** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contrast-security": {
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
