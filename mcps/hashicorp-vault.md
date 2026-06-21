# HashiCorp Vault MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hashicorp-vault)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Securely manage secrets, tokens, and encryption keys via HashiCorp Vault — read KV secrets, generate dynamic credentials, and monitor system health.

## Description
Connect your **HashiCorp Vault** instance to any AI agent to automate secrets management and security operations through natural language.

### What you can do

- **Secrets Management** — Read, write, and list KV secrets directly from your secure mounts using the KV engine.
- **Dynamic Credentials** — Generate on-demand credentials for Databases, AWS, and PKI certificates without manual intervention.
- **Token Operations** — Create, lookup, and renew tokens to manage session lifecycles and access control.
- **Transit Encryption** — Encrypt and decrypt data using Vault's transit engine to protect sensitive information without exposing keys.
- **System Administration** — Check cluster health, manage mounts, and configure auth methods or ACL policies directly.

### How it works

1. Subscribe to this server
2. Provide your Vault Address and Token
3. Start managing your infrastructure security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate secret rotation and infrastructure provisioning workflows.
- **Security Teams** — audit token accessors and manage ACL policies through conversation.
- **Developers** — fetch development secrets and generate local database credentials without leaving the IDE.


## Available Tools (50)
- **approle_login**: Login using AppRole authentication
- **configure_aws_root**: Configure AWS root credentials
- **configure_database**: Configure a database connection
- **configure_kubernetes_auth**: Configure Kubernetes authentication
- **create_acl_policy**: Create or update an ACL policy
- **create_approle_role**: Create or update an AppRole role
- **create_aws_role**: Create an AWS role
- **create_database_role**: Create a database role
- **create_pki_role**: Create a PKI role
- **create_token**: Create a new Vault token
- **create_transit_key**: Create a new Transit key
- **create_userpass_user**: Create a new Userpass user
- **decrypt_transit**: Decrypt data using Transit engine
- **delete_kv_secret**: Delete the latest version of a KV v2 secret
- **enable_audit_device**: Enable an audit device
- **enable_auth_method**: Enable a new auth method
- **enable_engine**: Enable a new secrets engine
- **encrypt_transit**: Encrypt data using Transit engine
- **generate_approle_secret_id**: Generate a new Secret ID for an AppRole
- **generate_aws_creds**: Generate dynamic AWS credentials
- **generate_database_creds**: Generate dynamic database credentials
- **generate_pki_root**: Generate a new PKI root certificate
- **get_init_status**: Check Vault initialization status
- **get_openapi_spec**: Generate OpenAPI V3 document of mounted backends
- **get_system_health**: Check Vault system health
- **github_login**: Login using GitHub personal access token
- **initialize_vault**: Initialize a new Vault cluster
- **issue_pki_cert**: Issue a new PKI certificate
- **kubernetes_login**: Login using Kubernetes authentication
- **list_acl_policies**: List ACL policies
- **list_audit_devices**: List enabled audit devices
- **list_auth_methods**: List enabled auth methods
- **list_kv_secrets**: List secrets in a KV v2 engine path
- **list_mounts**: List mounted secrets engines
- **list_token_accessors**: List token accessors (requires sudo)
- **lookup_lease**: Lookup a lease by ID
- **lookup_self_token**: Lookup details about the current Vault token
- **map_github_team**: Map a GitHub team to Vault policies
- **read_kv_metadata**: Read metadata for a KV v2 secret
- **read_kv_secret**: Read a secret from KV v2 engine
- **renew_lease**: Renew a lease
- **renew_self_token**: Renew the current Vault token
- **revoke_lease**: Revoke a lease
- **revoke_pki_cert**: Revoke a PKI certificate
- **revoke_self_token**: Revoke the current Vault token
- **rotate_transit_key**: Rotate a Transit key
- **seal_vault**: Seal the Vault
- **unseal_vault**: Unseal the Vault with a key share
- **userpass_login**: Login using Username and Password
- **write_kv_secret**: Create or update a secret in KV v2 engine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HashiCorp Vault** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the health and initialization status of my Vault server."

**🤖 AI Agent:**
> I've checked the system. The Vault server is initialized and unsealed. Health check returned 200 OK with version 1.15.2.

---

**👤 You:**
> "Read the secret stored at 'secret/data/production/api-keys'."

**🤖 AI Agent:**
> I've retrieved the secret. It contains 2 keys: `STRIPE_KEY` and `AWS_SECRET_ACCESS_KEY`. Would you like me to display the values?

---

**👤 You:**
> "Renew my current Vault token for another hour."

**🤖 AI Agent:**
> The token has been successfully renewed. The new lease duration is 3600 seconds.


## ❓ FAQ

**Q: Can I check the remaining TTL and policies of my current session token?**
Yes. Use the `lookup_self_token` tool. It returns the creation time, TTL, associated policies, and metadata for the token currently in use.

**Q: How do I retrieve a specific secret from a KV version 2 engine?**
Use the `read_kv_secret` tool by providing the path to the secret. The agent will fetch the data and present the key-value pairs securely.

**Q: Is it possible to generate temporary database credentials through the agent?**
Yes. If the database engine is configured, use `generate_database_creds` with the specific role name to receive a temporary username and password.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashicorp-vault](https://vinkius.com/mcp/hashicorp-vault)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HashiCorp Vault** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hashicorp-vault` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HashiCorp Vault** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hashicorp-vault": {
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
