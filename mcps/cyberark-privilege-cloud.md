# CyberArk Privilege Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cyberark-privilege-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cyberark-privilege-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cyberark-privilege-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage privileged access via CyberArk — audit secure safes, checkout vaulted account passwords, monitor users, and terminate sessions directly from any AI agent.

## Description
Connect your **CyberArk Privilege Cloud** account to any AI agent and take full control of your identity security and privileged access management through natural conversation.

### What you can do

- **Safe Orchestration** — List secure Safes and retrieve intricate settings including retention periods and assigned Central Policy Managers (CPM)
- **Privileged Account Management** — Enumerate vaulted credentials (Root, Administrator, Service Accounts) and audit rotational statuses and address mappings
- **Password Retrieval (Check-out)** — Pull actual secrets from the Vault with mandatory audited justifications, allowing the agent to securely retrieve credentials for incident response
- **Identity Oversight** — List internal and LDAP-mapped directory users and groups to verify PAM logical access architectures and RBAC rules
- **Session Control** — Forcibly terminate active PSM/PSMP privileged sessions instantly as an active incident response mechanism
- **Vault Onboarding** — Provision new privileged accounts into secure Safes by mapping them to specific platform IDs for automated rotation lifecycle management

### How it works

1. Subscribe to this server
2. Enter your CyberArk Subdomain and your Bearer access_token (generated via a Service User client_credentials flow)
3. Start managing your privileged access from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts & SOC** — monitor privileged account status and terminate suspicious sessions in real-time
- **IT Administrators** — onboard new service accounts and manage safe configurations without navigating the PVWA interface
- **Auditors & Compliance** — list users, groups, and account properties to verify organizational security policies
- **DevOps Engineers** — retrieve temporary credentials for automated maintenance tasks with full audit logging


## Available Tools
- **add_account**: Requires precise mapping to an underlying Platform ID (e.g., WinDesktopLocal, UnixSSH) which dictates how CyberArk rotates and verifies the credential moving forward.

Provision a new privileged account into a Vault Safe
- **delete_account**: Requires high authorization. Used during system decommissioning so the CPM stops attempting failed password rotations.

Delete a privileged account from the CyberArk Vault
- **get_account**: Necessary before rotating or interacting with an account.

Get detailed properties for a specific vaulted account
- **get_safe**: Get details and metadata for a specific PAM Safe
- **list_accounts**: These represent highly sensitive credentials (Root, Administrator, Service Accounts). Includes the bounding platform, Safe allocation, address, and rotational status. Use the search string to narrow targets.

Search and list privileged accounts vaulted in CyberArk
- **list_groups**: Permissions to Safes are canonically granted to Groups rather than individual users to enforce RBAC best practices. Used to verify PAM logical access architectures.

List CyberArk Vault User Groups
- **list_safes**: Safes are the fundamental logical containers separating credentials physically and logically. Required to locate where specific critical tier-0 credentials or local admin passwords reside.

List all secure Safes in CyberArk Privileged Access Manager
- **list_users**: Identifies active vault administrators, auditors, and human end-users consuming PSM (Privileged Session Manager) sessions.

List all CyberArk users (local and synchronized)
- **retrieve_password**: Highly audited endpoint triggering SIEM alerts. A justification reason is mandatory. After retrieval, exclusive access platforms may lock the credential until check-in or auto-rotation.

Retrieve the clear-text password for an account (check-out)
- **terminate_session**: Used as an active incident response mechanism if a SOC analyst or anomalous behavior engine detects unauthorized actions mid-session.

Forcibly terminate an active Privileged Session (PSM/PSMP)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CyberArk Privilege Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all privileged accounts for address '10.0.0.1'"

**🤖 AI Agent:**
> I found 2 accounts for '10.0.0.1': 'Root' (ID: 123) and 'Admin' (ID: 456). Both are in the 'Linux-Servers' Safe and their passwords were last rotated 5 days ago.

---

**👤 You:**
> "Retrieve password for account 123. Reason: 'Emergency DB maintenance'"

**🤖 AI Agent:**
> Password retrieved successfully! For account 123 (Root), the password is: '********'. This action has been logged with your justification. Would you like me to check-in the account once you are done?

---

**👤 You:**
> "Terminate active session 'sess_abc'"

**🤖 AI Agent:**
> Session 'sess_abc' has been forcibly terminated! The connection was cut instantly on the CyberArk PSM. The user has been disconnected from the target system.


## Installation & Usage

To install and use the **CyberArk Privilege Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cyberark-privilege-cloud](https://vinkius.com/mcp/cyberark-privilege-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
