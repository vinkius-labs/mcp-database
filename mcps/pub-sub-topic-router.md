# Pub-Sub Topic Router MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pub-sub-topic-router)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic routing engine for hierarchical topic patterns and wildcard subscriptions.

## Description
This MCP server provides a deterministic routing engine for managing hierarchical message delivery. It allows AI agents to calculate exact matching subscribers using wildcard patterns like `*` for single levels and `#` for multi-level matching. Use `match_subscribers` to identify targets, `calculate_delivery_impact` to evaluate traffic and QoS guarantees, and `analyze_topic_complexity` to inspect topic depth and expansion potential. It is designed to manage fanout impact and back-pressure in complex agent communication networks.


## Available Tools (3)
- **analyze_topic_complexity**: Inspects the structure of a topic to determine routing complexity and expansion potential
- **calculate_delivery_impact**: Evaluates the resource requirements and guarantees for a single message publication
- **match_subscribers**: Identifies which specific agents should receive a message published to a specific topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pub-Sub Topic Router** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all subscribers for the topic 'agents.planner.tasks.high' with these subscriptions: [{'agentId': 'agent_1', 'topicPattern': 'agents.#'}, {'agentId': 'agent_2', 'topicPattern': 'agents.*.tasks.*'}]"

**🤖 AI Agent:**
> The matching subscribers are agent_1 and agent_2. The total fanout count is 2.

---

**👤 You:**
> "Calculate the delivery impact for a 500 byte message on topic 'sensor.temp' with QoS level 1 and matching subscribers: [{'agentId': 'sub_1', 'queueSize': 50, 'isOnline': true}]"

**🤖 AI Agent:**
> The delivery guarantee is at least once. Total traffic is 500 bytes. No back-pressure is needed.

---

**👤 You:**
> "Analyze the complexity of the topic 'a.b.c.d' with patterns ['a.#', 'a.*.c.*']"

**🤖 AI Agent:**
> The topic depth is 4. The expansion count for the provided patterns is 2.


## ❓ FAQ

**Q: How does wildcard matching work?**
The router uses `*` to match exactly one level in a hierarchy and `#` to match all remaining levels.

**Q: What is the maximum topic depth supported?**
The system supports a maximum topic depth of 10 levels.

**Q: How is back-pressure handled?**
If a subscriber's queue exceeds 1000 messages, the `calculate_delivery_impact` tool flags that back-pressure is needed to slow down the publisher.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pub-sub-topic-router](https://vinkius.com/ai-agent-connect/pub-sub-topic-router)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pub-Sub Topic Router** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pub-sub-topic-router` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pub-Sub Topic Router** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pub-sub-topic-router": {
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
