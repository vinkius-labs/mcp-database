# UpGuard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upguard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Monitor your attack surface and assess vendor security risks with continuous scanning that identifies vulnerabilities before attackers do.

## Description
Connect your **UpGuard** account to any AI agent and simplify how you monitor your attack surface, assess third-party vendor risks, and protect your organization's digital assets through natural conversation.

### What you can do

- **Vendor Risk Assessment** — List and query all monitored vendors to retrieve their security scores and metadata.
- **Risk Monitoring** — List active security risks detected across your own infrastructure (BreachSight) and your vendor network (VendorRisk).
- **Data Breach Tracking** — Monitor identity breaches affecting your workforce and retrieve detailed breach reports.
- **Asset Visibility** — List monitored domains, IP ranges, and SaaS applications to understand your digital footprint.
- **Employee Security** — Audit user-related risk data and identity theft exposures directly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your UpGuard API Key (found in your account settings)
3. Start managing your cybersecurity posture from Claude, Cursor, or any MCP client

### Who is this for?

- **CISO & Security Analysts** — quickly check security scores and identify critical infrastructure risks via simple AI queries.
- **Procurement & Compliance** — verify vendor risk profiles and monitor third-party security posture directly from the workspace.
- **IT Operations** — track monitored domains and IPs to maintain a secure and up-to-date asset inventory.


## Available Tools
- **get_vendor**: Get details for a specific vendor
- **list_saas_apps**: List monitored SaaS applications
- **list_identity_breaches**: List identity breaches
- **list_monitored_domains**: List monitored domains
- **list_monitored_ips**: List monitored IP addresses
- **list_account_risks**: List all active risks for the account
- **list_user_risks**: List users and their risk data
- **list_vendor_risks**: List active risks for a vendor
- **list_vendors**: List all monitored vendors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UpGuard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitored vendors and their security scores."

**🤖 AI Agent:**
> I've retrieved your vendor list. You are monitoring 15 vendors. Top scorers include 'Cloud Analytics' (950/950) and 'Payment Gateway X' (920/950). 'Old Legacy Supplier' has a lower score of 450. Which one would you like a detailed risk report for?

---

**👤 You:**
> "Show me the active risks for the vendor 'Microsoft'."

**🤖 AI Agent:**
> I've fetched the risks for Microsoft. There are 2 active findings: 'Unencrypted backup found' and 'TLS 1.0 support detected'. Shall I retrieve the remediation steps for these?

---

**👤 You:**
> "Are there any recent identity breaches affecting our domain?"

**🤖 AI Agent:**
> Inspecting breach data... I found one recent identity breach affecting 3 employees. It occurred on a third-party site 'TrainingPortal.com'. Would you like the list of affected email addresses?


## ❓ FAQ

**Q: How do I check the security score of a specific vendor?**
Use the `get_vendor` tool and provide the Vendor ID. Your agent will retrieve the complete security profile, including the overall score and metadata for that vendor.

**Q: Can I see all active risks across my entire account?**
Yes! Use the `list_account_risks` query. This retrieves all active security risks detected across your own digital infrastructure (BreachSight).

**Q: Is it possible to monitor data breaches affecting our employees?**
Absolutely. Use the `list_identity_breaches` query to retrieve data on identity breaches affecting your workforce, helping you take proactive security measures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upguard](https://vinkius.com/mcp/upguard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UpGuard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `upguard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UpGuard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upguard": {
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
