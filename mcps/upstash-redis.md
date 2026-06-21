# Upstash Redis MCP Server

Equip your AI to directly query, manage, and manipulate key-value data structures inside your serverless Upstash Redis databases.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/upstash-redis)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Connect your **Upstash Redis** serverless database securely to your conversational AI agent via their REST API. Activating this integration grants your AI the technical autonomy to function as a responsive database administrator, enabling it to scan live keys, read raw datastore strings, set temporal expiration values, and even debug in real-time straight from your chat or IDE terminal.

### What you can do

- **Read & Write Values** — Fetch the exact string configuration of a stored key (`get`), or instruct the AI to inject a new value (`set`) complete with Time-To-Live (TTL) expiration limits.
- **Data Structure Discovery** — Perform pattern-based scans across your database to track down dynamically generated keys and inspect their underlying structures or lifespans (`list_keys`, `get_key_info`).
- **Manage Counters** — Safely increment or decrement numerical keys dynamically, perfect for managing rate limits, operational counters, or user session metrics directly during troubleshooting flows.
- **Maintain Health** — Ping the cluster instance for responsive status checks and remove (`delete`) specific keys or cache fragments completely.

### How it works

1. Authorize the Upstash Redis MCP component in your active module extensions.
2. Obtain both the `REST URL` and `REST Token` connected to your intended database from your Upstash console and submit them in the configuration fields.
3. Chat natively with your AI to prompt a scan of cache items like 'session:*' or adjust active TTLs on a throttling profile.

### Who is this for?

- **Backend Developers** — Verify cache hits, clear outdated session states intuitively, or seed temporary mock parameters rapidly without launching specialized desktop database clients like RedisInsight.
- **DevOps Engineers** — Inspect the rate-limiting structures or increment manual counter matrices safely during live-site debugging incidents.
- **System Architects** — Audit temporal key lifespans testing new eviction behaviors immediately as they write operational code logic.


## Available Tools
- **delete**: Provide a comma-separated list of keys.

Deletes one or more keys from Redis
- **get**: Retrieves the string value stored at a key
- **increment**: Use negative numbers to decrement.

Increments or decrements a numeric counter at a key
- **get_key_info**: Retrieves the data type and TTL of a key
- **list_keys**: Avoid broad patterns like "*" on large databases.

Scans for keys matching a glob pattern
- **ping**: Pings the Redis instance to verify connectivity
- **set**: You can specify expiry in seconds.

Sets a string value at a key with an optional TTL


## Installation & Usage

To install and use the **Upstash Redis** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upstash-redis](https://vinkius.com/mcp/upstash-redis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
