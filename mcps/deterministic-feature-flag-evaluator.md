# Deterministic Feature Flag Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-feature-flag-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Evaluate feature flags using consistent, hash-based logic to prevent session flicker.

## Description
The Deterministic Feature Flag Evaluator provides a reliable way to manage feature rollouts without the risk of inconsistent user experiences. By utilizing CRC32 hashing on the combination of a flag key and a user ID, it ensures that a user's assignment to a feature remains stable across different sessions and agents. This MCP server allows you to use `evaluate_flag` to check if a specific user meets rollout criteria, `verify_distribution` to validate the uniformity of your percentage-based rollouts, and `get_flag_config` to retrieve existing rule definitions from the registry. It is an essential tool for maintaining feature consistency in multi-agent environments like Cursor, VS Code, and Claude Desktop.


## Available Tools (3)
- **evaluate_flag**: Evaluates if a feature flag is enabled for a specific user
- **get_flag_config**: Retrieves the configuration for a given flag key
- **verify_distribution**: Verifies if the flag distribution is uniform across a sample size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Feature Flag Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'user_123' is enabled for the 'new_ui_v2' flag with a 50% rollout."

**🤖 AI Agent:**
> The evaluation for user 'user_12im' on flag 'new_ui_v2' resulted in: isEnabled: true, evaluationReason: PERCENTAGE, hashValue: 42.

---

**👤 You:**
> "Retrieve the configuration for the 'beta_search' flag."

**🤖 AI Agent:**
> The configuration for 'beta_search' was found: configExists: true, rules: {"percentageRollout": 25, "allowedIds": ["admin_01"]}.

---

**👤 You:**
> "Verify if a 10% rollout for 'dark_mode' is uniform using a sample of 1000 users."

**🤖 AI Agent:**
> The distribution test completed: observedPercentage: 10.2, deviationFromExpected: 0.2, isWithinTolerance: true.


## ❓ FAQ

**Q: How does the system ensure a user doesn't see a feature flicker?**
The system uses CRC32 hashing of the `flagKey` and `userId`. Since these inputs are immutable for a specific user and flag, the resulting hash value remains constant, ensuring the feature state does not change between sessions.

**Q: Can I bypass the percentage rollout for specific users?**
Yes. By providing an `allowedIds` list within the `rulesJson` parameter of the `evaluate_flag` tool, you can explicitly enable a feature for specific users regardless of the percentage rollout.

**Q: How do I verify if my rollout is actually distributed correctly?**
You can use the `verify_distribution` tool. By specifying a target percentage and a sample size, the tool will simulate users and report if the observed distribution matches your expected rollout percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-feature-flag-evaluator](https://vinkius.com/mcp/deterministic-feature-flag-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Feature Flag Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-feature-flag-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Feature Flag Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-feature-flag-evaluator": {
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
