# Fly.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flyio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flyio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flyio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage edge infrastructure via Fly.io — monitor apps and machines, scale compute horizontally, handle persistent volumes, and run remote commands directly from any AI agent.

## Description
Connect your **Fly.io** account to any AI agent and take full control of your edge computing and container orchestration through natural conversation.

### What you can do

- **App Space Orchestration** — List logical parent containers (Apps) spanning the Fly Edge network, identifying anycast assignments and dedicated IPv4/IPv6 IPs natively
- **Machine Runtime Management** — Navigate and control individual MicroVM (Machine) endpoints, fetching unique IDs and explicit placement regions flawlessly
- **Autonomous Scaling** — Provision new highly available Edge Machines to scale horizontal capacities dynamically without waiting on full platform deployments
- **Live Health Auditing** — Examine exhaustive runtime states, returning dynamic executing statuses (started, stopped, suspended) and docker image digests in real-time
- **Remote Command Execution** — Inject and run shell commands inside active Machines bypassing SSH by interacting directly with the hypervisor API securely
- **Persistent Storage Control** — List hardware NVMe Volumes attached to your apps to manage stateful data like PostgreSQL or SQLite independent of compute
- **Network DNA Extraction** — Retrieve the operational baseline of Fly Apps, identifying Wireguard ranges and cluster master regions synchronously

### How it works

1. Subscribe to this server
2. Enter your Fly.io API Token (found in Fly.io Dashboard > Account > Tokens or via `fly auth token`)
3. Start managing your edge infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Platform Engineers** — monitor machine health and scale horizontally across global regions using natural language
- **Backend Developers** — trigger restarts, run database migrations, and verify deployment digests directly from the chat
- **Cloud Architects** — audit anycast IP assignments and persistent volume mappings without manual CLI commands
- **SRE Teams** — monitor system execution logs and run diagnostic commands on active machines in real-time


## Available Tools
- **create_machine**: Scales horizontal capacities dynamically without waiting on full platform deployments.

Provision a new highly available Edge Machine inside an App
- **delete_machine**: The Firecracker VM is dropped, compute billing ceases immediately, and any ephemeral disk state dissolves. Fails safely if persistent volumes are explicitly attached without the force flag.

Terminate and destroy a Fly Machine forever (Scale Down)
- **exec_machine**: Useful for `ls`, `ps aux`, `top`, or running internal database diagnostic migrations.

Inject and run a shell/Bash command inside an active Fly Machine
- **get_app**: Identifies the primary Region holding the cluster master, internal Wireguard network ranges assigned, and any active Anycast IPs actively routing inbound user traffic globally.

Retrieve the operational baseline state of a distinct Fly App
- **get_machine**: Returns dynamic executing states ("started", "stopped", "suspended"), the precise docker image digest/SHA actively booted into RAM, and any mapped volume points tying persistent SQLite/Postgres logs.

Get exhaustive runtime states attached to a single Fly Machine
- **list_apps**: Apps are fundamentally distinct collections of individual microVMs (Machines), dedicated IPv4/IPv6 anycast assignments, and persistent storage volumes.

List Fly.io App spaces belonging to an Organization
- **list_machines**: Retrieves unique identifiers and explicit placement Regions (e.g., iad, ams, nrt).

List individual MicroVM (Machine) endpoints inside a Fly App
- **list_volumes**: Crucial identifier for managing stateful applications (PostgreSQL, SQLite, persistent cache) safely independent of compute instances.

List persistent hardware NVMe Volumes attached to an App
- **start_machine**: Utilized extensively when recovering paused batch processors or restarting crashed worker nodes dynamically across edge points of presence.

Boot a previously stopped or suspended Fly Machine
- **stop_machine**: Drastically reduces latency bills during idle cycles outside typical user ingress bands.

Gracefully halt a running Fly.io internal Machine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fly.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all machines in my 'web-api' app"

**🤖 AI Agent:**
> Retrieving machines... I found 2 machines in 'web-api': '918572b0' (Region: iad, Status: started) and 'e28654c1' (Region: gru, Status: stopped). Would you like me to start the stopped machine?

---

**👤 You:**
> "Run 'ls -la /app' on machine '918572b0' in app 'web-api'"

**🤖 AI Agent:**
> Command execution initiated! I've sent the request to machine 918572b0. Result: [Detailed directory listing showing files in /app folder]. No SSH required, I used the Fly Machine API synchronously.

---

**👤 You:**
> "Show me the persistent volumes for 'web-api'"

**🤖 AI Agent:**
> Retrieving volumes... I found 1 persistent NVMe volume: 'data_vol' (Size: 10GB, Region: iad). It is currently attached to machine 918572b0 and is residency on physical hardware node xyz.


## Installation & Usage

To install and use the **Fly.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flyio](https://vinkius.com/mcp/flyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
