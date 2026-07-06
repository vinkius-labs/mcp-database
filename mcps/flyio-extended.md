# Fly.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flyio-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Fly.io apps, machines, and infrastructure—provision resources, control machine lifecycles, and manage volumes directly from any AI agent.

## Description
Connect your **Fly.io** account to any AI agent to orchestrate your cloud infrastructure through natural language. This server provides full access to the Fly Machines API, allowing for granular control over global deployments.

### What you can do

- **App Management** — Create, list, and delete Fly Apps across your organizations.
- **Machine Lifecycle** — Start, stop, suspend, and update individual Machines with precise configuration control.
- **Storage & Volumes** — Provision, extend, and manage persistent volumes and snapshots for your stateful applications.
- **Network & Security** — Manage ACME and custom certificates, and request OIDC tokens for secure workload identity.
- **Real-time Monitoring** — Wait for specific machine states and fetch detailed metadata for debugging and orchestration.

### How it works

1. Subscribe to this server
2. Enter your Fly.io Personal Access Token
3. Start deploying and managing your global infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Automate scaling, machine restarts, and volume management without leaving the terminal or chat interface.
- **Full-stack Developers** — Deploy new app instances and check machine statuses directly from your code editor.
- **SRE Teams** — Quickly inspect infrastructure health and manage certificates during incident response.


## Available Tools (28)
- **create_lease**: Create a lease for a Machine
- **create_machine**: Requires a config object containing at least the image.

Create a new Fly Machine
- **create_volume**: Create a new volume
- **delete_app**: Delete a Fly App
- **delete_certificate**: Remove hostname and certificates
- **delete_machine**: Delete a Machine
- **delete_volume**: Delete a volume
- **extend_volume**: Increase volume size
- **get_app**: Get details about a Fly App
- **get_certificate**: Get certificate details
- **get_machine**: Get Machine details
- **get_volume**: Get volume details
- **list_apps**: List Fly Apps
- **list_certificates**: List all certificates for an app
- **list_machines**: List all Machines in an app
- **list_volume_snapshots**: List volume snapshots
- **list_volumes**: List all volumes in an app
- **release_lease**: Release a lease for a Machine
- **request_oidc_token**: Request an OpenID Connect (OIDC) token
- **start_machine**: Start a Machine
- **stop_machine**: Stop a Machine
- **suspend_machine**: Suspend a Machine
- **update_machine**: Update Machine configuration
- **wait_machine**: Wait for a specific Machine state
- **check_certificate**: Trigger DNS validation check for a certificate
- **create_acme_certificate**: Request a Let's Encrypt certificate
- **create_app**: Create a new Fly App
- **create_custom_certificate**: Import a custom PEM certificate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fly.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Fly.io apps in the 'personal' organization."

**🤖 AI Agent:**
> I've retrieved your apps for the 'personal' organization. You have 3 active apps: 'my-api-server', 'web-frontend-prod', and 'db-primary'. Would you like to see the machines running in any of these?

---

**👤 You:**
> "Start the machine with ID 9185210b6e4d8p in the app 'my-api-server'."

**🤖 AI Agent:**
> Starting machine 918... The request was successful. The machine is now transitioning to the 'started' state.

---

**👤 You:**
> "Create a 10GB volume named 'data_vol' in the 'ams' region for app 'db-primary'."

**🤖 AI Agent:**
> I've initiated the creation of a 10GB volume 'data_vol' in Amsterdam (ams) for 'db-primary'. The volume ID is vol_z9rj5k2m1l. It is now ready to be attached to a machine.


## ❓ FAQ

**Q: Can I start or stop a specific Fly Machine using this server?**
Yes. You can use the `start_machine` and `stop_machine` tools by providing the app name and the specific Machine ID. You can also use `suspend_machine` for compatible workloads.

**Q: How do I create a new application in a specific organization?**
Use the `create_app` tool. You will need to provide a unique `app_name` and the `org_slug` of the target organization where you want the app to be provisioned.

**Q: Is it possible to manage persistent storage volumes?**
Absolutely. The server includes tools like `create_volume`, `list_volumes`, `extend_volume`, and `delete_volume` to handle the full lifecycle of your Fly Volumes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flyio-extended](https://vinkius.com/mcp/flyio-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fly.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flyio-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fly.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flyio-extended": {
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
