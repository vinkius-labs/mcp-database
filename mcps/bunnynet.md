# Bunny.net MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bunnynet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bunnynet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bunnynet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Bunny.net edge infrastructure — control your CDN Pull Zones, purge caching rules, and map Storage natively from an AI agent.

## Description
Connect your **Bunny.net** platform to any AI agent and operate your edge CDN and cloud storage entirely through natural conversation.

### What you can do

- **Pull Zones Management** — View and create ultra-fast reverse proxy acceleration links that distribute your media globally
- **Cache Invalidations** — Instantly purge the cache on specific CDN zones, pushing out immediate changes and breaking TTLs
- **Edge Storage Clusters** — Analyze or delete raw origin volumes routing permanent data arrays
- **File Exploration** — Inspect precise static payloads directly inside the CDN Edge Storage structure via FTP parameters

### How it works

1. Subscribe to this server
2. Enter your master Bunny API Key and standard zone tokens
3. Start managing your Edge structure from Claude, Cursor, or any MCP-compatible smart client

No clunky network portals or messy CURL commands. Your AI agent becomes your core Edge configuration wizard.

### Who is this for?

- **DevOps Engineers** — burst edge configurations, destroy stale proxies, and debug origin faults rapidly
- **Front-End Devs** — purge cache immediately after code deployment guaranteeing users hit fresh Javascript bundles
- **Media Content Owners** — track files deep within origin edge storages seamlessly routing video uploads


## Available Tools
- **add_pull_zone**: Returns the new Pull Zone ID and default b-cdn.net domain.

Provision a radically fast new CDN reverse proxy domain
- **add_storage_zone**: Defaults to explicit NY regional primary datacenters.

Bootstrap an entirely empty replication Volume inside Bunny.net
- **delete_pull_zone**: Instantly invalidates assigned `b-cdn.net` aliases dropping incoming proxy connections out of the Anycast caching tree entirely.

Destroy an active CDN acceleration mapping terminating global traffic
- **delete_storage_zone**: Requires zone to be empty or forces recursive wipes freeing the namespace back into the registry.

Vaporize an existing Bunny CDN Storage Zone entirely
- **get_pull_zone**: Exposes enabled SSL configurations, Bandwidth limits, and advanced Edge Rules intercepting requests.

Perform structural extraction of metadata for one specific Pull Zone
- **get_storage_zone**: Returns FTP access credentials, read-only vs read-write keys, and origin PoPs.

Inspect deep internal credentials identifying a precise Storage Zone
- **list_files**: Requires the specific Zone FTP/API Password. Returns literal byte lengths and cryptographic hash footprints.

Enumerate explicitly uploaded binary assets nested strictly inside Storage
- **list_pull_zones**: Returns pull zone IDs, names, hostnames, and origin URL targets.

Identify global Bunny CDN accelerated delivery domains (Pull Zones)
- **list_storage_zones**: Locate physical Edge Storage origin folders managed natively on Bunny
- **purge_pull_zone**: Spikes Origin ingress traffic rapidly pulling entirely fresh payload structures.

Blast an immediate Cache Invalidation forcing origin asset re-fetching


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bunny.net** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Pull Zones and their original targets."

**🤖 AI Agent:**
> You have 2 Pull Zones explicitly active. ID 12040 runs 'prod-app-cdn' targeting your AWS S3 bucket. ID 19302 runs 'staging-cdn' pointing to your beta server IP. Do you need to examine their advanced security configurations?

---

**👤 You:**
> "My site design looks old, the JS didn't update. Purge Pull Zone ID 12040 right now."

**🤖 AI Agent:**
> I've sent the global invalidation command. The CDN cache on Pull Zone 12040 has been instantly purged. Your edge nodes are now re-fetching the JS origin bundles actively. You're good to go.

---

**👤 You:**
> "What files are currently inside the '/assets/' path of our 'main-storage-x' Edge Storage zone?"

**🤖 AI Agent:**
> I checked your NVMe edge cluster. Within '/assets/', I found 'hero_bg.webp' (1.2 MB) and 'compiled_main.css' (900 KB). Shall I provide the cryptographic checksums?


## Installation & Usage

To install and use the **Bunny.net** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bunnynet](https://vinkius.com/mcp/bunnynet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
