# Okta MCP Server

Equip your AI agent with Okta Identity Cloud to manage users, groups, and seamless authentication effortlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/okta)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Okta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/okta](https://vinkius.com/mcp/okta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
