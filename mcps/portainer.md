# Portainer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portainer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/portainer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/portainer-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Portainer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portainer](https://vinkius.com/mcp/portainer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
