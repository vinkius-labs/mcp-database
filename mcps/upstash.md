# Upstash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upstash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage serverless Redis via Upstash REST API — execute commands, manage data structures and monitor your database from any AI agent.

## Description
Connect your **Upstash** Redis database to any AI agent and interact with your serverless data store through natural conversation — no Redis CLI needed.

### What you can do

- **Health Checks** — Ping your database to verify connectivity and inspect server health
- **String Operations** — Get, set and delete key-value pairs with optional TTL management
- **Hash Management** — Store and retrieve structured data as field-value pairs within hash keys
- **List Operations** — Push, pop and range elements from Redis lists for queue and stack patterns
- **Set Operations** — Add, remove and query set membership for unique collections
- **Key Discovery** — List keys by pattern, check existence, inspect data types and view TTL values
- **Numeric Operations** — Increment and decrement counters atomically
- **Pub/Sub Messaging** — Publish messages to channels for event-driven architectures
- **Pipeline Execution** — Execute multiple commands in a single HTTP request for batch operations

### How it works

1. Subscribe to this server
2. Enter your Upstash REST URL and Token
3. Start managing your Redis data from Claude, Cursor, or any MCP-compatible client

No more switching to another terminal to run Redis commands. Your AI acts as an in-memory data engineer.

### Who is this for?

- **Backend Developers** — manage caching layers, feature flags, session storage and rate limit counters directly from chat
- **DevOps Engineers** — monitor database health, audit key patterns and manage TTL-based data lifecycle
- **Full-Stack Teams** — manipulate data structures (hashes, lists, sets) for application state without opening Redis CLI


## Available Tools (23)
- **decr**: If the key does not exist, it is initialized to 0 before the operation. Returns the new value after decrementing.

Decrement a numeric value in Upstash Redis
- **del**: Returns 1 if the key was deleted, 0 if it did not exist. WARNING: this operation is irreversible.

Delete a key from Upstash Redis
- **exists**: This is a lightweight way to check key presence without retrieving the value.

Check if a key exists in Upstash Redis
- **expire**: The key will be automatically deleted when the TTL reaches zero. Returns 1 if the timeout was set, 0 if the key does not exist.

Set a TTL on a key in Upstash Redis
- **get**: Returns null if the key does not exist. This is the primary read operation for string data.

Get a value from Upstash Redis
- **hget**: Returns null if the key or field does not exist.

Get a field value from a Redis hash
- **hgetall**: Returns an object with all fields and their values. Returns an empty object if the key does not exist.

Get all fields and values from a Redis hash
- **hset**: If the key does not exist, a new hash is created. If the field already exists, its value is overwritten. Returns the number of fields added (1 for new, 0 for updated).

Set a field in a Redis hash
- **incr**: If the key does not exist, it is initialized to 0 before the operation. Returns the new value after incrementing.

Increment a numeric value in Upstash Redis
- **list_keys**: Use "*" for all keys, "prefix:*" for keys with a prefix, or "*:suffix" for suffix matching. WARNING: KEYS can be slow on large databases — use sparingly.

List keys in Upstash Redis
- **llen**: Returns 0 if the key does not exist.

Get the length of a Redis list
- **lpush**: If the key does not exist, a new list is created. Returns the length of the list after the push.

Push values to the left of a Redis list
- **lrange**: Use 0 as start and -1 as stop to get all elements. Positive indices count from the head (0 = first), negative indices count from the tail (-1 = last).

Get a range of elements from a Redis list
- **pipeline**: Commands are sent as a JSON array of arrays, e.g. [["SET","k1","v1"],["GET","k1"],["INCR","counter"]]. Returns an array of results in the same order. Note: the pipeline is NOT atomic (other commands may interleave) — use /multi-exec for atomicity. WARNING: this is a powerful tool — review commands carefully before execution.

Execute multiple commands atomically via Upstash pipeline
- **publish**: Returns the number of subscribers that received the message. This is a fire-and-forget operation — subscribers must be actively listening.

Publish a message to a Redis channel
- **rpush**: If the key does not exist, a new list is created. Returns the length of the list after the push.

Push values to the right of a Redis list
- **sadd**: Duplicate members are ignored. If the key does not exist, a new set is created. Returns the number of members that were added.

Add members to a Redis set
- **set**: Optionally set an expiry time in seconds using the ex parameter. Overwrites any existing value at the key. Returns "OK" on success. This is the primary write operation for string data.

Set a value in Upstash Redis
- **sismember**: This is a fast O(1) membership check.

Check if a member is in a Redis set
- **smembers**: Returns an array of all unique members. Returns an empty array if the key does not exist.

Get all members of a Redis set
- **srem**: Non-existent members are ignored. Returns the number of members that were removed.

Remove members from a Redis set
- **ttl**: Returns -1 if the key has no expiry, -2 if the key does not exist.

Get the TTL of a key in Upstash Redis
- **key_type**: Get the data type of a key in Upstash Redis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upstash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my Upstash Redis database is responding."

**🤖 AI Agent:**
> Connection verified! The database responded with PONG. Your Upstash Redis instance is healthy and accepting commands.

---

**👤 You:**
> "Set a feature flag called 'dark_mode' to true for user 'user123' with a 1 hour expiry."

**🤖 AI Agent:**
> Done! I've set the key `dark_mode:user123` to `true` with a 3600-second (1 hour) expiry. The flag will automatically expire after that time.

---

**👤 You:**
> "Show me all keys matching the pattern 'session:*' and check their data types."

**🤖 AI Agent:**
> I found 5 keys matching 'session:*'. Checking their types: `session:abc` is a hash, `session:def` is a hash, `session:ghi` is a string, `session:jkl` is a set, and `session:mno` is a list. Most sessions are stored as hashes (field-value pairs for user data).


## ❓ FAQ

**Q: Where do I find my Upstash REST URL and Token?**
Log in to the [**Upstash Console**](https://console.upstash.com), select your Redis database, and look for the **REST API** section. You'll find the HTTPS Endpoint (your REST URL, e.g. `https://xxx-yyy-12345.upstash.io`) and the **Token** value. Copy both and paste them here. There are two token types: Standard (full access) and Read-Only (read-only commands). Use Standard for full functionality.

**Q: What Redis commands are supported via the REST API?**
The Upstash REST API supports most Redis commands including: Strings (GET, SET, DEL, EXISTS, EXPIRE, TTL, INCR, DECR), Hashes (HSET, HGET, HGETALL), Lists (LPUSH, RPUSH, LRANGE, LLEN), Sets (SADD, SMEMBERS, SISMEMBER, SREM), Keys (KEYS, TYPE, PING), and Pub/Sub (PUBLISH). The pipeline endpoint allows executing multiple commands in a single request. Blocking commands (BLPOP, BRPOP) and WATCH/UNWATCH are not supported.

**Q: Can I execute multiple commands atomically?**
The `pipeline` tool sends multiple commands in a single HTTP request for efficiency, but it is NOT atomic — other commands may interleave between them. For atomic multi-command execution, Upstash supports the `/multi-exec` endpoint (same syntax as pipeline but guarantees atomicity). However, this MCP server currently exposes the standard pipeline tool for batch operations.

**Q: Is the Upstash REST API rate-limited?**
Upstash does not enforce a fixed RPS limit. Instead, your plan defines a daily command limit. Each REST call counts as one command (or multiple commands if using pipeline). If you exceed your daily limit, commands will fail with a 400 error. Check your Upstash console for current usage. For high-throughput scenarios, consider using the pipeline endpoint to batch multiple commands into single HTTP requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upstash](https://vinkius.com/mcp/upstash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upstash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upstash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upstash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upstash": {
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
