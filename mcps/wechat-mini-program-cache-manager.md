# WeChat Mini-Program Cache Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wechat-mini-program-cache-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministic WeChat Mini-Program storage and LRU cache eviction calculator.

## Description
This MCP server provides deterministic tools for managing WeChat Mini-Program local storage. It helps developers ensure compliance with platform-specific limits (10240 KB or 20480 KB) by calculating available space and simulating Least Recently Used (LRU) eviction. Use `calculate_storage_status` to check if a new item fits, `simulate_lru_eviction` to identify which items to remove based on their `last_access_timestamp`, and `get_cache_inventory` to audit current cache contents.


## Available Tools (3)
- **get_cache_inventory**: Provides a summary of the current cache contents to verify the state before performing calculations
- **calculate_storage_status**: Determines the current state of the cache and whether there is enough room to add a specific new item without triggering eviction
- **simulate_lru_eviction**: Calculates exactly which items must be removed to accommodate a new item using the LRU logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Mini-Program Cache Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if I can add a 500KB item to my cache which currently has 10000KB used out of 10240KB."

**🤖 AI Agent:**
> No, the new item will exceed the limit. You need to evict items to free up at least 500KB.

---

**👤 You:**
> "Show me the current cache inventory."

**🤖 AI Agent:**
> The current cache contains 5 items with a total size of 8500 KB.

---

**👤 You:**
> "Simulate eviction for a 2000KB item when the cache is at 10000/10240KB."

**🤖 AI Agent:**
> To accommodate the 2000KB item, the system will evict 2 items, freeing 2100KB of space.


## ❓ FAQ

**Q: How does the LRU eviction logic work?**
The system identifies items with the oldest `last_access_timestamp` and removes them sequentially until the new item fits within the specified `max_limit_kb`.

**Q: What are the standard WeChat cache limits?**
Limits are typically 10240 KB for standard environments or 20480 KB for extended capacity environments.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wechat-mini-program-cache-manager](https://vinkius.com/ai-agent-connect/wechat-mini-program-cache-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeChat Mini-Program Cache Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wechat-mini-program-cache-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeChat Mini-Program Cache Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wechat-mini-program-cache-manager": {
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
