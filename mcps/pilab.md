# PiLAB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pilab)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Manage infrastructure and security via PiLAB — control PiVirt virtual machines, inspect PiTrust certificates, and oversee 3SO OAuth clients directly from any AI agent.

## Description
Connect your **PiLAB** account to any AI agent and take full control of your infrastructure and security operations through natural conversation.

### What you can do

- **Virtual Machine Management** — List all PiVirt hosts, inspect VMs (CPU, memory, disk, network), and control lifecycle (start, stop, restart, pause, resume) from your chat
- **Certificate Management** — List all TLS/SSL certificates managed by PiTrust, inspect certificate metadata, chains, and rotation status
- **ZeroTrust Access Policies** — List RBAC rules, JIT access grants, and service-to-service authentication policies configured in PiTrust
- **OAuth 2.0 Client Management** — List all registered applications in 3SO (Shadow SSO), inspect client configurations, scopes, and grant types
- **Token Introspection** — Validate any OAuth 2.0 access token via the 3SO introspection endpoint (RFC 7662) to verify scopes and expiry
- **Session Monitoring** — List active user sessions in the 3SO identity system to audit who is authenticated and what scopes they hold

### How it works

1. Subscribe to this server
2. Register an OAuth 2.0 application in your PiLAB SSO admin console (one-time setup, ~5 minutes)
3. Enter your Client ID and Client Secret, then click **Connect with PiLAB** to authorize access
4. Start managing your infrastructure from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated infrastructure and security operations assistant — no more switching between the PiVirt console, PiTrust dashboard, and SSO admin panel to check a VM status or verify a certificate.

### Who is this for?

- **DevOps Engineers** — check VM status, control lifecycle, and verify host resources without leaving the conversation
- **Security Teams** — audit certificate expiries, inspect access policies, and verify token validity in real-time
- **Platform Architects** — review OAuth client configurations and active sessions to understand the identity landscape
- **IT Operations** — combine VM control with certificate monitoring for end-to-end infrastructure visibility


## Available Tools (12)
- **control_vm**: Valid actions: start, stop, restart, pause, resume. Use this to manage VM lifecycle from your AI agent.

Start, stop, or restart a virtual machine
- **get_certificate_details**: Get details for a specific certificate
- **get_host_details**: Get details for a specific PiVirt host
- **list_virtual_machines**: Optionally filter by host ID to see only VMs on a specific host.

List all virtual machines across PiVirt hosts
- **get_oauth_client**: Get details for a specific OAuth 2.0 client
- **get_vm_details**: Get details for a specific virtual machine
- **introspect_token**: Returns token validity, scopes, expiry, and associated client/user. Use this to verify tokens before trusting them.

Introspect an OAuth 2.0 access token
- **list_certificates**: List all TLS/SSL certificates managed by PiTrust
- **list_hosts**: List all PiVirt virtualization hosts
- **list_oauth_clients**: List all registered OAuth 2.0 clients
- **list_access_policies**: List all ZeroTrust access policies
- **list_active_sessions**: List active user sessions in the 3SO identity system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PiLAB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all virtual machines across my PiVirt hosts."

**🤖 AI Agent:**
> Retrieved 8 VMs across 3 hosts. Notable machines include 'web-prod-01' (running, host node-01), 'db-replica-02' (running, host node-02), and 'staging-api' (stopped, host node-03). Would you like details or to control any specific VM?

---

**👤 You:**
> "Start the VM with ID vm-1024."

**🤖 AI Agent:**
> Sent the 'start' command to VM vm-1024. The VM is now in 'running' state on host node-02. CPU: 4 vCPUs, Memory: 16 GB. Is there anything else you'd like to do with this VM?

---

**👤 You:**
> "Show me all TLS certificates and flag any that are expiring soon."

**🤖 AI Agent:**
> Found 6 certificates in PiTrust. ⚠️ Two need attention: '*.pilab.hu' expires in 12 days (rotation pending), and 'api.internal.pilab.hu' expires in 30 days. The remaining 4 certificates have at least 60 days before expiry. Would you like the full details on either expiring certificate?


## ❓ FAQ

**Q: How do I connect my PiLAB account?**
After subscribing, the setup wizard will guide you through 3 simple steps: 1) Enter your PiLAB Instance Base URL. 2) Enter the Client ID and Client Secret from your PiLAB SSO (3SO) application. 3) Click the **Connect with PiLAB** button — a popup will open where you approve access via the Shadow SSO authorization flow. That's it! No manual token exchange or curl commands required.

**Q: Where do I find the Redirect URI for my PiLAB SSO application?**
When registering your application in the PiLAB SSO admin console, set the **Redirect URI** to: `https://api.vinkius.com/marketplace/oauth/callback`. This is the platform's secure callback endpoint that completes the OAuth authorization automatically.

**Q: How do I get my Client ID and Client Secret?**
Sign in to your PiLAB SSO admin console at `https://sso.pilab.hu/primary/` and navigate to **Client Management**. Click **New Application**, give it a name, and set the **Redirect URI** to `https://api.vinkius.com/marketplace/oauth/callback`. Save the app and copy the **Client ID** and **Client Secret** (the secret is shown only once — copy it immediately).

**Q: Can my AI control virtual machines on PiVirt?**
Yes! Use `list_virtual_machines` to see all VMs, `get_vm_details` to inspect a specific VM's resources, and `control_vm` with actions like start, stop, restart, pause, or resume. Your AI can manage the full VM lifecycle from the conversation.

**Q: How do I check if a TLS certificate is about to expire?**
Use the `list_certificates` tool to see all certificates managed by PiTrust with their expiry dates and rotation status. For a specific certificate, use `get_certificate_details` with the certificate ID to see the full chain and rotation policy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pilab](https://vinkius.com/mcp/pilab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PiLAB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pilab` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PiLAB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pilab": {
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
