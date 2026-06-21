# Ping Identity MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ping-identity)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ping-identity-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ping-identity-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage PingOne user identities, applications, groups, risk policies, and sign-on flows autonomously via AI.

## Description
Connect your **Ping Identity** environment to any AI agent to streamline identity and access management (IAM). You can audit users, check security policies, and review applications directly through conversation.

### What you can do

- **User Management** — List identities, view detailed user profiles, and safely delete users across the enterprise directory.
- **Applications & Groups** — Audit all Web, Native, or SPA apps federated under your environment, and list active IAM groups.
- **Populations** — Review isolated populations dividing contractors, partners, or B2B clients.
- **Risk & Policies** — Inspect active Risk Management rules and Zero-Trust sign-on workflows dictating real-time MFA.

### How it works

1. Subscribe to this server
2. Enter your PingOne Environment ID and API Token
3. Start managing your enterprise identity posture from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IAM Administrators** — audit active user populations, access groups, and verify application settings faster.
- **Security Engineers** — review real-time risk policies, sign-on flows, and MFA requirements instantly without navigating consoles.
- **IT Support** — quickly fetch specific user metadata and check active session/credential health.


## Available Tools
- **delete_user**: Revokes all current session tokens, nullifies application scopes, isolates SCIM directory references, and executes the formal deletion API.

Hard delete a user identity and purge related credentials
- **get_application**: Determines configured Implicit/Authorization Code grants, token lifespan definitions, embedded sign-on policies, and allowed callback URIs required for stringent redirection security mapping.

Get configuration for a single federated Ping Identity application
- **get_group**: View explicit details encompassing a standard Ping Group
- **get_user**: Get complete contextual metadata for a specific Ping Identity user
- **list_applications**: Crucial to verify application exposure footprint.

List Web, Native or SPA apps federated under standard PingOne
- **list_groups**: Allows mapping high-level RBAC scopes dynamically injected into ID tokens returned via SSO channels upon successful client authorization flows.

List identity Groups utilized for aggregate permissions
- **list_populations**: g., 'Contractors', 'Partners', 'B2B Clients') possessing inherently different default password complexities, independent password expiration parameters, and isolated self-service recovery scopes.

List isolated Populations logically partitioning the Environment
- **list_users**: Paginates across all bounded external and internal localized users containing primary credentials, deeply nested JSON identifiers, and physical verification states assigned under the Enterprise Directory schema.

List all user identities within the standard PingOne Environment
- **list_risk_policies**: Evaluates contextual IP anomalies, impossible travel, blocklisted VPN routes, or behavioral irregularities explicitly stepping up authentication flows or directly blocking malicious login execution.

List active Risk Management rules dictating real-time MFA
- **list_sign_on_policies**: Sign-on policies chain distinct rules together enforcing explicit MFA prompts, enforcing complex password structures based on population assignment, or mandating implicit biometric validation prior to releasing environment tokens.

List logical Sign-on flows and strict authentication conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ping Identity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you list all OIDC applications configured in PingOne and highlight any insecure callbacks?"

**🤖 AI Agent:**
> You currently have 8 configured applications. I noticed that 'Legacy CRM' uses an Implicit Grant and lacks PKCE. Also, 'Staging Dashboard' has a callback URI using a non-secure protocol (`http://`). I recommend modifying these components directly in the admin console to maintain Zero-Trust compliance.

---

**👤 You:**
> "Provide the active list of Zero-Trust risk policies governing my environment."

**🤖 AI Agent:**
> There are 3 active Risk Policies in your designated execution environment. 
1. **Impossible Travel** — triggers mandatory MFA prompts upon anomalous geographic location jumps.
2. **Anonymous Networks** — drops authentication directly for identified VPN and TOR entry-points.
3. **Behavior Anomalies** — triggers a step-up challenge utilizing Ping's machine-learning baseline models.
What would you like to drill down into?

---

**👤 You:**
> "Delete the specific suspended user profile assigned to the ID `81773-XYZ-192`."

**🤖 AI Agent:**
> Execution successful. The PingOne distinct identity assigned to `81773-XYZ-192` has been removed explicitly. Associated explicit MFA linkages, secondary sessions, isolated SCIM references, and assigned app scopes have all been safely purged from the Directory.


## Installation & Usage

To install and use the **Ping Identity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ping-identity](https://vinkius.com/mcp/ping-identity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
