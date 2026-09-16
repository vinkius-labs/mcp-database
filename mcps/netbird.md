# NetBird MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/netbird)
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


## Available Tools (89)
- **list_setup_keys**: Use this tool to view existing one-off or reusable keys.

List all setup keys
- **approve_user**: Provide the user ID of the account to activate.

Approve a pending user
- **change_user_password**: Supply the user ID and the new password payload.

Change user password (embedded IdP only)
- **create_group**: Supply the necessary group details in the body payload.

Create a group
- **create_msp_tenant**: Pass the required details in the body payload.

Create a new MSP tenant
- **create_nameserver**: Supply the required details in the body payload.

Create a nameserver group
- **create_network_resource**: Supply the network ID and the resource details.

Create a resource (host, subnet, or domain) in a network
- **create_network_router**: Provide the necessary router details in the body.

Create a router in a network
- **create_policy**: The policy details must be provided in the body.

Create a policy with rules (action, protocol, ports, sources, destinations)
- **create_posture_check**: Provide a valid JSON payload in the body.

Create a posture check (version, OS, geo-location, network range, or process)
- **create_route**: Supply the necessary route details in the body payload.

Create a route (Deprecated)
- **create_setup_key**: Specify the key type and payload in the body. Use this for provisioning.

Create a setup key (one-off or reusable)
- **create_temporary_access_peer**: Supply a valid peer_id and the necessary access payload.

Create a temporary access peer
- **create_user_invite**: Supply the necessary invite details in the body payload.

Create a user invite link
- **create_user_token**: Supply the user ID and payload.

Create a new personal access token
- **create_user**: Provide a valid user payload in the body.

Create a service user or invite a regular user
- **delete_account**: Provide the account ID to execute the deletion.

Delete a NetBird account and all resources
- **delete_group**: Supply the group ID to execute the deletion.

Delete a group
- **delete_nameserver**: Ensure the Nameserver Group ID is correct.

Delete nameserver group
- **delete_network_resource**: Supply the network ID and the resource ID to confirm deletion.

Delete network resource
- **delete_network_router**: Ensure the router ID and network ID are correct.

Delete network router
- **delete_policy**: Use the policy ID to target the policy for deletion.

Delete a policy
- **delete_route**: Ensure the provided Route ID is correct.

Delete a route (Deprecated)
- **delete_user_token**: Supply the user ID and token ID.

Delete a token
- **get_current_user**: This retrieves details for the authenticated user.

Retrieve current user info
- **get_dns_settings**: Retrieve global DNS settings
- **get_group**: Use a valid group_id to fetch the group information.

Retrieve group details
- **get_nameserver**: Use the Nameserver Group ID.

Retrieve nameserver group details
- **get_network_resource**: Supply both the network and resource IDs.

Retrieve network resource details
- **get_network_router**: Must provide both the network and router identifiers.

Retrieve network router details
- **get_network**: Use the network ID for identification.

Retrieve network details
- **get_peer**: Provide the peer ID.

Retrieve peer details
- **get_policy**: Use the policy ID to target the correct policy.

Retrieve policy details
- **get_posture_check**: Use a valid Posture Check ID.

Retrieve posture check details
- **get_public_user_invite**: The token must be provided.

Get public invite info (unauthenticated)
- **get_route**: Provide a valid Route ID.

Retrieve route details (Deprecated)
- **get_setup_key**: Pass the specific Setup Key ID to retrieve information.

Retrieve setup key details
- **get_user_token**: Provide both the user ID and token ID.

Retrieve a specific token
- **invite_msp_tenant**: Requires the tenant ID and invite details.

Invite an existing account as a tenant
- **list_accounts**: Do not use this tool to list individual users.

List all NetBird accounts
- **list_all_network_routers**: List all routers across all networks
- **list_audit_events**: List all audit events (activity, initiator, target)
- **list_cities**: Provide the country’s ISO 3166-1 alpha-2 code.

List city names for a country
- **list_countries**: List all ISO 3166-1 alpha-2 country codes
- **list_groups**: Use this tool to list available network groups.

List all groups
- **list_nameservers**: List all nameserver groups
- **list_network_resources**: Provide the network ID to scope the search.

List resources in a network
- **list_network_routers**: Requires a valid network ID.

List routers in a network
- **list_networks**: Do not provide any parameters.

List all networks
- **list_peers**: Use this tool to list connected devices and nodes.

List all network peers
- **list_posture_checks**: List all posture checks
- **list_routes**: Note that this tool is deprecated.

List all routes (Deprecated)
- **list_user_tokens**: Requires the user ID.

List all tokens for a user
- **list_users**: Use this tool to retrieve a list of all registered users.

List all users
- **regenerate_user_invite**: Use the invite ID.

Regenerate an invite token
- **reject_user**: Provide the user ID of the account to reject.

Reject a pending user
- **resend_user_invite**: Use the user ID to target the correct recipient.

Resend user invitation
- **respond_msp_tenant_invite**: Requires the tenant ID and response payload.

Accept or decline an MSP invitation
- **update_account**: Pass the account ID and the settings payload.

Update account settings (e.g., peer login expiration, network range)
- **update_group**: Provide the group ID and the necessary JSON payload.

Update group name, peers, or resources
- **update_msp_tenant_subscription**: Provide the tenant ID and subscription payload.

Create/update tenant subscription
- **update_msp_tenant**: Provide the tenant ID and update details in the body.

Update tenant name or access groups
- **update_network_resource**: Provide the network ID, resource ID, and update payload.

Update network resource
- **update_network**: Specify the network ID and the update payload.

Update network name/description
- **update_peer**: Provide a valid peer_id in the request body.

Update peer name, SSH status, or IP
- **update_policy**: Provide the policy ID and the new configuration body.

Update policy
- **update_posture_check**: Supply the Posture Check ID and update payload.

Update posture check
- **update_route**: Supply both the Route ID and the update payload.

Update route (Deprecated)
- **update_setup_key**: Provide the Setup Key ID and the new payload.

Update key (revoke or change auto-groups)
- **update_user**: Supply the user ID and the update payload.

Update user role, auto-groups, or block status
- **accept_user_invite**: Supply the token and required payload.

Accept invite and set password (unauthenticated)
- **list_accessible_peers**: Use a valid peer_id to query the list.

List peers accessible by this peer
- **update_nameserver**: Supply the Nameserver Group ID and update payload.

Update nameserver group
- **verify_msp_tenant_dns**: Requires the tenant ID.

Verify tenant domain DNS challenge
- **create_network**: Pass the required details in the JSON payload.

Create a network
- **delete_network**: Provide the network ID to confirm deletion.

Delete a network
- **delete_peer**: Ensure the peer_id is correct to prevent accidental deletion.

Delete a peer
- **delete_posture_check**: Ensure the Posture Check ID is correct.

Delete a posture check
- **list_network_traffic_events**: Note that this feature is experimental and cloud-only.

List network traffic events (Cloud-only, experimental)
- **list_user_invites**: List pending user invites
- **unlink_msp_tenant**: Requires the tenant ID.

Unlink a tenant to a new owner
- **update_dns_settings**: Pass a JSON payload in the body.

Update DNS settings (e.g., disabled management groups)
- **update_network_router**: Use the router ID and network ID for targeting.

Update network router
- **delete_setup_key**: Specify the Setup Key ID to permanently remove the key.

Delete a setup key
- **delete_user_invite**: Provide the unique invite ID.

Delete a user invite
- **delete_user**: Specify the user ID to ensure the correct account is deleted.

Remove a user
- **list_msp_tenants**: List all MSP tenants
- **list_policies**: List all policies
- **list_proxy_events**: List reverse proxy access logs


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


## ❓ FAQ

**Q: How can I see all users currently registered in my NetBird network?**
You can use the `list_users` tool. It will return a complete list of users, including their IDs, roles, and current status.

**Q: Is it possible to invite a new user to the network via AI?**
Yes! Use the `create_user_invite` tool to generate an invitation link, or `create_user` to invite a regular user directly by providing the necessary JSON payload.

**Q: Can I manage pending user approvals through this integration?**
Absolutely. Use `approve_user` to grant access to a pending user or `reject_user` to deny their request using their specific User ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/netbird](https://vinkius.com/en/ai-agent-connect/netbird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NetBird** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `netbird` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NetBird** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netbird": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
