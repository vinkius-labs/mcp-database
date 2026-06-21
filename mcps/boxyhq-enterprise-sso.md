# BoxyHQ (Enterprise SSO) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boxyhq-enterprise-sso)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage Enterprise SSO and Directory Sync (SCIM) via BoxyHQ — configure SAML/OIDC connections and automate user provisioning directly from your AI agent.

## Description
Connect your **BoxyHQ** instance to any AI agent to streamline enterprise authentication and user lifecycle management through natural language.

### What you can do

- **SSO Connections** — Add, update, and manage SAML and OIDC connections for specific tenants and products.
- **Directory Sync (SCIM)** — Create and configure SCIM 2.0 directories to automate user provisioning and de-provisioning.
- **Connection Auditing** — Retrieve detailed connection metadata using tenant IDs, product IDs, or client IDs.
- **Metadata Management** — Configure IdP metadata via raw XML (Base64) or direct metadata URLs for rapid deployment.
- **Lifecycle Control** — Update existing security configurations or delete stale connections to maintain a clean security posture.

### How it works

1. Subscribe to this server
2. Enter your BoxyHQ Instance URL and API Key
3. Start managing enterprise identity workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — quickly audit and update SSO configurations across multiple tenants without manual dashboard navigation.
- **DevOps & SREs** — automate the creation of SCIM directories and SAML connections during customer onboarding.
- **Product Managers** — verify the status of enterprise integrations and connection health directly from the chat interface.


## Available Tools
- **add_connection**: Add a new SAML or OIDC connection
- **create_directory**: 0 protocol.

Create a Directory Sync (SCIM) connection
- **delete_connection**: Delete an SSO connection
- **get_connections**: Get SSO connections
- **get_directory_groups**: List all groups for a tenant/product directory
- **get_directory_users**: List all users for a tenant/product directory
- **health_check**: Check BoxyHQ service health
- **update_connection**: Update an existing SSO connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoxyHQ (Enterprise SSO)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a new SAML connection for tenant 'acme.com' and product 'saas-app' using metadata URL 'https://idp.com/metadata.xml'."

**🤖 AI Agent:**
> I've successfully created the SAML connection for acme.com. The Client ID is `conn_abc123`. You can now use this for SSO authentication.

---

**👤 You:**
> "List all SSO connections for the product 'enterprise-portal'."

**🤖 AI Agent:**
> I found 3 connections for 'enterprise-portal': 'Globex Corp' (SAML), 'Initech' (OIDC), and 'Umbrella' (SAML). Which one would you like to inspect?

---

**👤 You:**
> "Create an Okta SCIM directory for tenant 'piedpiper' and product 'cloud-storage'."

**🤖 AI Agent:**
> The Okta SCIM directory for piedpiper has been created. SCIM Base URL: `https://sso.boxyhq.com/api/scim/v2.0/piedpiper`. Please provide this to the customer to start syncing users.


## ❓ FAQ

**Q: Can I configure a SAML connection using just the metadata URL?**
Yes! Use the `add_connection` tool and provide the `metadataUrl`. The server will fetch and process the IdP configuration automatically.

**Q: How do I find the clientID for an existing connection?**
You can use the `get_connections` tool by providing the `tenant` and `product` IDs. It will return all matching connections including their unique clientIDs.

**Q: Does this support SCIM for automated user provisioning?**
Absolutely. Use the `create_directory` tool to set up a SCIM 2.0 directory for providers like Okta, Azure AD, or Google, including webhook support for events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boxyhq-enterprise-sso](https://vinkius.com/mcp/boxyhq-enterprise-sso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoxyHQ (Enterprise SSO)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `boxyhq-enterprise-sso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoxyHQ (Enterprise SSO)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boxyhq-enterprise-sso": {
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
