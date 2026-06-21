# UpGuard MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upguard)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/upguard-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/upguard-mcp)
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


## Installation & Usage

To install and use the **UpGuard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upguard](https://vinkius.com/mcp/upguard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
