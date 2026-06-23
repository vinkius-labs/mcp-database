# Portainer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portainer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Docker containers and environments via Portainer — list, create, and start containers directly from your AI agent.

## Description
Connect your **Portainer** instance to any AI agent and orchestrate your containerized infrastructure through natural conversation.

### What you can do

- **Container Management** — List all Docker containers in any environment, create new ones from images, and start existing containers.
- **Environment Orchestration** — Add and manage new local or remote Docker/Kubernetes environments (endpoints) to your Portainer setup.
- **Admin Control** — Initialize admin accounts on fresh installations and authenticate to receive secure JWT tokens.
- **Configuration Control** — Deploy containers with custom configurations, including exposed ports and host settings via JSON.

### How it works

1. Subscribe to this server
2. Enter your Portainer URL and API Key
3. Start managing your devops infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check container statuses and restart services without leaving the terminal or chat.
- **Developers** — deploy new testing environments or images directly from the code editor.
- **System Administrators** — manage multiple remote environments and endpoints through a unified AI interface.


## Available Tools (6)
- **add_endpoint**: Add a new environment (endpoint) to Portainer
- **authenticate**: Authenticate to receive a JWT token
- **create_docker_container**: Create a new Docker container
- **init_admin**: Initialize Portainer admin password
- **list_docker_containers**: List Docker containers in an environment
- **start_docker_container**: Start a Docker container


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portainer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all containers in Portainer endpoint 1."

**🤖 AI Agent:**
> I've retrieved the container list for endpoint 1. You have 4 containers: 'nginx-proxy' (running), 'db-postgres' (running), 'redis-cache' (stopped), and 'app-worker' (running).

---

**👤 You:**
> "Create a new container named 'web-server' using the 'nginx:latest' image in endpoint 2."

**🤖 AI Agent:**
> The container 'web-server' has been successfully created in endpoint 2 using the nginx:latest image. Would you like me to start it now?

---

**👤 You:**
> "Start the container 'redis-cache' in endpoint 1."

**🤖 AI Agent:**
> Starting 'redis-cache' in endpoint 1... The container has been started successfully.


## ❓ FAQ

**Q: How do I see all containers running in a specific environment?**
Use the `list_docker_containers` tool by providing the specific `endpoint_id`. The agent will return a list of all containers managed within that Portainer environment.

**Q: Can I add a new remote Docker endpoint through the AI?**
Yes! Use the `add_endpoint` action. You can specify the name, set the type to 2 (Remote), and provide the URL (e.g., tcp://10.0.0.1:2375) to connect a new environment.

**Q: Is it possible to deploy a container with specific port mappings?**
Yes. When using `create_docker_container`, you can provide a `config_json` string containing standard Docker API parameters like `ExposedPorts` or `HostConfig` to define your network and port requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portainer](https://vinkius.com/mcp/portainer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portainer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portainer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portainer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portainer": {
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
