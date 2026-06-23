# Upstash Redis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upstash-redis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI to directly query, manage, and manipulate key-value data structures inside your serverless Upstash Redis databases.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upstash Redis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Redis keys associated with app sessions."

**🤖 AI Agent:**
> I invoked the `list_keys` query with the pattern 'session:*'. Found 3 active keys residing in your environment.

---

**👤 You:**
> "Check the Time-To-Live duration limit configured for the 'cache:product_header' key."

**🤖 AI Agent:**
> I checked the key info via `get_key_info`. The 'cache:product_header' value is a standard String and currently holds a remaining Time-to-Live format of exactly 3600 seconds.

---

**👤 You:**
> "Delete all caching strings tagged as 'user_193_avatar' from the database immediately."

**🤖 AI Agent:**
> Using the `delete` tool, I have entirely removed the 'user_193_avatar' cache key structure from the Upstash datastore instance. Future calls seeking this key limit will return null entries until regenerated.


## ❓ FAQ

**Q: Where do I locate my Upstash REST URL and Token?**
Sign into your Upstash management console and load your specific Redis cluster. Scroll down visually on the main 'Details' page until you hit the 'REST API' section block. You will see both your 'UPSTASH_REDIS_REST_URL' and the alphanumeric 'UPSTASH_REDIS_REST_TOKEN' ready to be copied.

**Q: Can the agent interact with standard Redis connections (redis://)?**
No, this specific MCP connection module specifically utilizes Upstash's serverless HTTP/REST endpoints. It bypasses conventional persistent TCP Redis sockets to provide highly secure and connection-agnostic read/write integrations optimized for AI servers.

**Q: Are there limitations to wildcard patterns when doing list_keys?**
Yes, standard Redis operational caveats apply. Searching broadly via a '*' (asterisk) scan across massively populated environments isn't recommended. Aim to request the AI narrow down patterns, like 'session:*' instead of blank wildcards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upstash-redis](https://vinkius.com/mcp/upstash-redis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upstash Redis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upstash-redis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upstash Redis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upstash-redis": {
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
