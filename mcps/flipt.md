# Flipt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flipt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage feature flags and rollouts via Flipt — list namespaces, flags, segments, and rules directly from your AI agent.

## Description
Connect your **Flipt** instance to any AI agent to orchestrate feature management and progressive delivery through natural conversation.

### What you can do

- **Flag Management** — List and inspect feature flags across different namespaces to understand your current feature states
- **Targeting & Segments** — Retrieve segments and create constraints to define specific user subsets for targeted rollouts
- **Rollout Control** — List rules and rollouts, and create distributions to manage percentage-based releases and canary deployments
- **Variants** — Create and manage flag variants to return different values based on evaluation logic
- **Auth & Infrastructure** — List authentication tokens and namespaces to understand your environment's structure and access levels

### How it works

1. Subscribe to this server
2. Enter your Flipt URL and API Token
3. Start managing your feature flags from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly audit rollout configurations and namespace partitions without leaving the terminal or IDE
- **Product Managers** — check the status of feature flags and segments to verify release progress
- **Developers** — create variants and constraints directly while coding to speed up feature implementation


## Available Tools (9)
- **create_constraint**: Create a constraint for a segment
- **create_distribution**: Create a distribution for a rule
- **create_variant**: Create a new variant for a flag
- **list_flags**: List flags in a namespace
- **list_namespaces**: List all namespaces
- **list_rollouts**: List rollouts for a flag
- **list_rules**: List rules for a flag
- **list_segments**: List segments in a namespace
- **list_tokens**: List authentication tokens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flipt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all namespaces in my Flipt instance."

**🤖 AI Agent:**
> I've retrieved the namespaces. You currently have: 'default' (Global resources) and 'production-env' (Production flags). Which one would you like to explore?

---

**👤 You:**
> "Show me all the feature flags in the 'default' namespace."

**🤖 AI Agent:**
> Fetching flags for 'default'... I found 3 flags: 'new-onboarding-flow', 'dark-mode-beta', and 'api-v2-enabled'. Would you like to see the variants for any of these?

---

**👤 You:**
> "Create a new variant called 'v2-test' for the 'header-experiment' flag in the 'default' namespace."

**🤖 AI Agent:**
> Variant 'v2-test' has been successfully created for the 'header-experiment' flag. It is now available for use in your rules and distributions.


## ❓ FAQ

**Q: Can I list all feature flags in a specific namespace?**
Yes! Use the `list_flags` tool and provide the `namespaceKey` (e.g., 'default'). The agent will return all flags configured within that partition.

**Q: How do I define a new variant for an existing flag?**
You can use the `create_variant` action. You'll need to specify the `namespaceKey`, `flagKey`, and the new variant's `key` and `name`.

**Q: Is it possible to see the rollout configuration for a specific flag?**
Absolutely. Use the `list_rollouts` tool by providing the target `namespaceKey` and `flagKey` to retrieve the current rollout strategy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flipt](https://vinkius.com/mcp/flipt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flipt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flipt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flipt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flipt": {
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
