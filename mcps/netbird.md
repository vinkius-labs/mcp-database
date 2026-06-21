# NetBird MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netbird)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/netbird-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/netbird-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Automate Zero Trust networking via NetBird — manage accounts, users, and access controls directly from any AI agent.

## Description
Connect your **NetBird** account to any AI agent and take full control of your private network infrastructure through natural conversation.

### What you can do

- **Account Management** — List and update account settings, including peer login expiration and network ranges using `list_accounts` and `update_account`.
- **User Administration** — Create service users, invite regular users, and manage roles or block statuses with `list_users`, `create_user`, and `update_user`.
- **Access Control** — Approve or reject pending users and manage user invitations efficiently using `approve_user` and `reject_user`.
- **Security & Identity** — Change user passwords for embedded IdP and retrieve current user information via `get_current_user` and `change_user_password`.
- **Invitation Workflow** — Generate, regenerate, and track user invite links to scale your network using `list_user_invites` and `create_user_invite`.

### How it works

1. Subscribe to this server
2. Enter your NetBird API Token
3. Start managing your Zero Trust network from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation to manage peer access or user onboarding. Your AI acts as a network administrator.

### Who is this for?

- **DevOps Engineers** — quickly manage network accounts and peer settings without leaving the terminal or IDE.
- **IT Administrators** — automate user onboarding, invitations, and access approvals through simple commands.
- **Security Teams** — monitor active users and manage security settings like password changes and account blocks instantly.


## Available Tools
- **accept_user_invite**: Accept invite and set password (unauthenticated)
- **approve_user**: Approve a pending user
- **change_user_password**: Change user password (embedded IdP only)
- **create_group**: Create a group
- **create_msp_tenant**: Create a new MSP tenant
- **create_nameserver**: Create a nameserver group
- **create_network_resource**: Create a resource (host, subnet, or domain) in a network
- **create_network_router**: Create a router in a network
- **create_network**: Create a network
- **create_policy**: Create a policy with rules (action, protocol, ports, sources, destinations)
- **create_posture_check**: Create a posture check (version, OS, geo-location, network range, or process)
- **create_route**: Create a route (Deprecated)
- **create_setup_key**: Create a setup key (one-off or reusable)
- **create_temporary_access_peer**: Create a temporary access peer
- **create_user_invite**: Create a user invite link
- **create_user_token**: Create a new personal access token
- **create_user**: Create a service user or invite a regular user
- **delete_account**: Delete a NetBird account and all resources
- **delete_group**: Delete a group
- **delete_nameserver**: Delete nameserver group
- **delete_network_resource**: Delete network resource
- **delete_network_router**: Delete network router
- **delete_network**: Delete a network
- **delete_peer**: Delete a peer
- **delete_policy**: Delete a policy
- **delete_posture_check**: Delete a posture check
- **delete_route**: Delete a route (Deprecated)
- **delete_setup_key**: Delete a setup key
- **delete_user_invite**: Delete a user invite
- **delete_user_token**: Delete a token
- **delete_user**: Remove a user
- **get_current_user**: Retrieve current user info
- **get_dns_settings**: Retrieve global DNS settings
- **get_group**: Retrieve group details
- **get_nameserver**: Retrieve nameserver group details
- **get_network_resource**: Retrieve network resource details
- **get_network_router**: Retrieve network router details
- **get_network**: Retrieve network details
- **get_peer**: Retrieve peer details
- **get_policy**: Retrieve policy details
- **get_posture_check**: Retrieve posture check details
- **get_public_user_invite**: Get public invite info (unauthenticated)
- **get_route**: Retrieve route details (Deprecated)
- **get_setup_key**: Retrieve setup key details
- **get_user_token**: Retrieve a specific token
- **invite_msp_tenant**: Invite an existing account as a tenant
- **list_accessible_peers**: List peers accessible by this peer
- **list_accounts**: List all NetBird accounts
- **list_all_network_routers**: List all routers across all networks
- **list_audit_events**: List all audit events (activity, initiator, target)
- **list_cities**: List city names for a country
- **list_countries**: List all ISO 3166-1 alpha-2 country codes
- **list_groups**: List all groups
- **list_msp_tenants**: List all MSP tenants
- **list_nameservers**: List all nameserver groups
- **list_network_resources**: List resources in a network
- **list_network_routers**: List routers in a network
- **list_network_traffic_events**: List network traffic events (Cloud-only, experimental)
- **list_networks**: List all networks
- **list_peers**: List all network peers
- **list_policies**: List all policies
- **list_posture_checks**: List all posture checks
- **list_proxy_events**: List reverse proxy access logs
- **list_routes**: List all routes (Deprecated)
- **list_setup_keys**: List all setup keys
- **list_user_invites**: List pending user invites
- **list_user_tokens**: List all tokens for a user
- **list_users**: List all users
- **regenerate_user_invite**: Regenerate an invite token
- **reject_user**: Reject a pending user
- **resend_user_invite**: Resend user invitation
- **respond_msp_tenant_invite**: Accept or decline an MSP invitation
- **unlink_msp_tenant**: Unlink a tenant to a new owner
- **update_account**: Update account settings (e.g., peer login expiration, network range)
- **update_dns_settings**: Update DNS settings (e.g., disabled management groups)
- **update_group**: Update group name, peers, or resources
- **update_msp_tenant_subscription**: Create/update tenant subscription
- **update_msp_tenant**: Update tenant name or access groups
- **update_nameserver**: Update nameserver group
- **update_network_resource**: Update network resource
- **update_network_router**: Update network router
- **update_network**: Update network name/description
- **update_peer**: Update peer name, SSH status, or IP
- **update_policy**: Update policy
- **update_posture_check**: Update posture check
- **update_route**: Update route (Deprecated)
- **update_setup_key**: Update key (revoke or change auto-groups)
- **update_user**: Update user role, auto-groups, or block status
- **verify_msp_tenant_dns**: Verify tenant domain DNS challenge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NetBird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my NetBird account."

**🤖 AI Agent:**
> I've retrieved the user list. You have 3 active users: Admin (ID: user_1), Developer A (ID: user_2), and Service_Bot (ID: user_3). Would you like to manage any of them?

---

**👤 You:**
> "Create a new user invite link."

**🤖 AI Agent:**
> I've generated a new invite link (ID: invite_abc123). You can share this with the new user to join your network.

---

**👤 You:**
> "Show me the details of the current authenticated user."

**🤖 AI Agent:**
> The current user is 'Admin' with email 'admin@company.com'. Your role is 'Owner' and you have full access to the account settings.


## Installation & Usage

To install and use the **NetBird** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netbird](https://vinkius.com/mcp/netbird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
