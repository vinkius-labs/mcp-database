# Fly.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flyio-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flyio-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flyio-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage edge compute infrastructure via Fly.io — list apps, control machines (VMs), manage volumes and certificates from any AI agent.

## Description
Connect your **Fly.io** account to any AI agent and take full control of your edge compute infrastructure through natural conversation.

### What you can do

- **App Management** — List all apps and retrieve their configuration details including regions, status and organization
- **Machine Lifecycle** — Create, start, stop, restart, update and delete machines (VMs) with full control over CPU, memory, region and image
- **Machine Inspection** — View machine state, configuration, services, health checks and IP addresses
- **Persistent Volumes** — List and create persistent storage volumes that survive machine restarts and redeployments
- **Certificate Management** — Review TLS/SSL certificates and their issuance status for app domains
- **Global Deployment** — Deploy machines across Fly.io's global regions (iad, sjc, nrt, fra, syd, etc.) for low-latency access

### How it works

1. Subscribe to this server
2. Enter your Fly.io Personal Access Token
3. Start managing your edge infrastructure from Claude, Cursor, or any MCP-compatible client

Stop using the CLI or web dashboard to manage individual VMs. Your AI acts as a dedicated edge infrastructure engineer.

### Who is this for?

- **Platform Engineers** — provision and manage VMs across multiple regions, scale services and monitor machine health without SSH
- **DevOps Teams** — inspect machine configurations, review deployments, manage persistent storage and track certificate status
- **Full-Stack Developers** — quickly check machine status, restart problematic VMs and verify image versions directly from chat


## Available Tools
- **create_machine**: io app. Requires the Docker image reference (e.g. "registry.fly.io/myapp:latest"). Optionally set the region (e.g. "iad", "sjc", "nrt"), CPU cores (1-16), memory in MB (256-8192), guest CPU kind (shared, performance) and services config. Machines start in stopped state — use start_machine after creation.

Create a new machine in a Fly.io app
- **create_volume**: Requires the volume name and size in gigabytes. Optionally set the region. The volume must be attached to a machine via the machine config mounts.

Create a persistent volume for a Fly.io app
- **delete_machine**: The machine cannot be recovered. Optionally set force=true to delete even if the machine has an attached volume. Provide the app_name and machine_id. WARNING: this action is irreversible.

Delete a Fly.io machine permanently
- **get_app**: io app including its name, status, regions, organization and network configuration. Provide the app name (not ID).

Get details for a specific Fly.io app
- **get_machine**: Provide both the app_name and machine_id.

Get details for a specific Fly.io machine
- **list_apps**: io account. Each app is a collection of machines (VMs) running your code across Fly.io's global edge network. Returns app name, status, region and creation date. Use the app name for all subsequent machine, volume and certificate operations.

List all Fly.io apps
- **list_certificates**: io app. Each certificate has a hostname, status (issued, pending, failed) and source (lets_encrypt, self_signed, acme). Use this to audit HTTPS certificate status for your app's domains.

List TLS/SSL certificates for a Fly.io app
- **list_machines**: io app. Each machine has an ID, name, state (started, stopped, created, destroyed), region, image reference, CPU/memory config and IP addresses. Machines are the fundamental compute units on Fly.io.

List machines (VMs) for a Fly.io app
- **list_volumes**: io app. Each volume has an ID, name, state, size in GB, region and the machine it is attached to. Volumes provide persistent storage that survives machine restarts.

List persistent volumes for a Fly.io app
- **restart_machine**: Useful for applying configuration changes or recovering from issues. Provide the app_name and machine_id.

Restart a Fly.io machine
- **start_machine**: The machine will boot and begin running its configured image. Provide the app_name and machine_id.

Start a stopped Fly.io machine
- **stop_machine**: The machine will stop and release its compute resources but retains its configuration and data. Provide the app_name and machine_id.

Stop a running Fly.io machine
- **update_machine**: You can modify the Docker image, CPU/memory allocation, services config, mounts and more. Provide the app_name, machine_id and a JSON body with the fields to update.

Update a Fly.io machine configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fly.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all machines running in my web-api app."

**🤖 AI Agent:**
> Your web-api app has 3 machines: 'web-api-1' in iad (started, 1 CPU, 512MB), 'web-api-2' in fra (started, 1 CPU, 512MB) and 'web-api-3' in nrt (stopped). All running image registry.fly.io/web-api:v2.1.0.

---

**👤 You:**
> "Start the stopped machine in Tokyo and restart the one in Frankfurt."

**🤖 AI Agent:**
> Done! I've started machine 'web-api-3' (nrt) — it's now booting. I've also restarted 'web-api-2' (fra) — it will stop and start again with its current configuration. Both machines should be healthy within a minute.

---

**👤 You:**
> "Create a new 10GB volume called 'data' for my database app in Virginia."

**🤖 AI Agent:**
> Done! I've created a 10GB persistent volume called 'data' in the iad (Virginia) region for your database app. The volume is ready to be attached to a machine via its mount configuration.


## Installation & Usage

To install and use the **Fly.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flyio-alternative](https://vinkius.com/mcp/flyio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
