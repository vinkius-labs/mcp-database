# Fly.io MCP Server

Manage edge infrastructure via Fly.io — monitor apps and machines, scale compute horizontally, handle persistent volumes, and run remote commands directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flyio)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Fly.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flyio](https://vinkius.com/mcp/flyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
