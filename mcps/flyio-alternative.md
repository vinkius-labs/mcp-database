# Fly.io MCP Server

Manage edge compute infrastructure via Fly.io — list apps, control machines (VMs), manage volumes and certificates from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flyio-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

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


## Installation & Usage

To install and use the **Fly.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flyio-alternative](https://vinkius.com/mcp/flyio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
