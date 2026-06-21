# Okta MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/okta)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/okta-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/okta-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with Okta Identity Cloud to manage users, groups, and seamless authentication effortlessly.

## Description
Connect your **Okta** Identity Cloud instance to any AI agent to streamline identity management, user provisioning, and secure access flows. Eliminate the need to dig through administrative dashboards by interacting conversationally to create users, unblock accounts, or manage group assignments.

### What you can do

- **User Provisioning & Lifecycle** — Interrogate the AI to list active users, retrieve specific profile details, create new identities, or cleanly deprovision departing employees
- **Access Control & Troubleshooting** — Instantly check a user's sign-in activity to resolve locks, reset credentials, or clear active sessions centrally
- **Group Segregation** — Manage departmental access by querying group directories, creating structured groups, or orchestrating bulk user assignments into logical access structures
- **Application Assignment** — Audit the integrations mapped to your user base, ensuring proper access to company apps based on the least-privilege principle

### How it works

1. Subscribe to this directory management server
2. Introduce your Okta domain and organizational API Key (SSWS)
3. Converse with your AI to perform administrative commands securely

### Who is this for?

- **IT & Helpdesk Teams** — Instantly unlock accounts, trigger password resets, or check group assignments bypassing complex administrator screens
- **Security Operations (SecOps)** — Trace individual sign-in scopes, terminate hazardous sessions, and audit assigned organizational apps rapidly
- **System Administrators** — Construct custom automated onboarding or offboarding commands dictating user lifecycles natively


## Available Tools
- **clear_user_sessions**: Necessary when a device is compromised.

Terminate all active login sessions for a specific user
- **deactivate_user**: This instantly converts the user status to DEPROVISIONED, permanently revoking all active sessions, killing SAML/OIDC assertions, and blocking future application access. Use for emergency offboarding.

Suspend and deprovision an Okta user account immediately
- **get_group**: View details of a specific Okta Group
- **get_user**: Input takes the explicit Okta User ID string.

Get detailed profile and state for a specific Okta user
- **get_app**: Includes critical security bindings, client secrets (for OIDC), X.509 cert chains, ACS URLs, and strict token-grant lifespans.

View detailed SSO configuration for a specific application
- **list_groups**: Group policies explicitly determine which users can authenticate into which bound SAML apps, making this endpoint critical for auditing permissions.

List all security, app, and dynamic Okta Groups
- **list_users**: Used for organization-wide identity reporting.

List all users configured in the Okta Universal Directory
- **list_system_logs**: Contains every discrete sign-in attempt, MFA challenge result, configuration tweak, and malicious password spraying anomaly. Max 100 recent entries.

Retrieve Recent Okta System and Audit log events
- **list_apps**: Identifies available sign-on integrations spanning raw OIDC, classical SAML 2.0, SCIM provisioning connections, and SWA (Secure Web Authentication) apps.

List all applications integrated within the Okta dashboard
- **list_group_users**: Essential when determining precisely who was automatically granted SCIM or cloud application licenses due to their directory membership mapping.

List all users currently assigned to an Okta Group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Okta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the user profile for 'mark@example.com'."

**🤖 AI Agent:**
> I found the profile for ID `00u12xxxxxxx`: Mark Johnson. The account status is currently `ACTIVE` and mapped to the 'Engineering' department. Would you like to check his group associations?

---

**👤 You:**
> "Clear all active sessions for user 'mike@example.com' immediately."

**🤖 AI Agent:**
> Success. I've sent the termination command to Okta. All active sessions for `mike@example.com` have been cleared and closed, forcing a re-login for any connected service.

---

**👤 You:**
> "List all active application mappings for the 'Contractors' group."

**🤖 AI Agent:**
> Scanning Group mapping ID `00xxxx` ('Contractors'): I found 3 provisioned apps tied to this cohort:
1. Slack (Provisioning Active)
2. Atlassian Jira Server (SAML)
3. Zoom (SAML)
Do you want me to revoke any permissions immediately?


## Installation & Usage

To install and use the **Okta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/okta](https://vinkius.com/mcp/okta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
