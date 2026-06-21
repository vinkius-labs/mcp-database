# Statsig MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statsig)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage feature flags, dynamic configs, and experiments. Evaluate gates and log events directly from your AI agent.

## Description
Connect your **Statsig** project to any AI agent to manage feature rollouts and product experiments through natural conversation.

### What you can do

- **Feature Gates** — Evaluate if a feature is enabled for a specific user or list all project gates
- **Dynamic Configs** — Fetch JSON configurations and experiments to control app behavior without code changes
- **Event Logging** — Log custom events for real-time analytics and metric calculation
- **Gate Management** — Create, update, or delete feature gates directly via the Console API
- **Layer Inspection** — Evaluate layers and retrieve parameter values for specific users

### How it works

1. Subscribe to this server
2. Enter your Statsig Server Secret Key (for evaluation) and Console API Key (for management)
3. Start managing your product experiments from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — check gate statuses and create new feature flags without leaving the chat
- **Developers** — verify evaluation logic and log test events directly from the IDE
- **Data Scientists** — inspect experiment configurations and verify metric logging


## Available Tools
- **check_gate**: Requires STATSIG_SERVER_SECRET_KEY.

Evaluates one or more feature gates for a user
- **create_dynamic_config**: Requires STATSIG_CONSOLE_API_KEY.

Create a new dynamic config
- **create_gate**: Requires STATSIG_CONSOLE_API_KEY.

Create a new feature gate
- **delete_gate**: Requires STATSIG_CONSOLE_API_KEY.

Delete a feature gate
- **get_config**: Requires STATSIG_SERVER_SECRET_KEY.

Fetches configuration values for a dynamic config or experiment
- **get_dynamic_config**: Requires STATSIG_CONSOLE_API_KEY.

Read a specific dynamic config
- **get_gate**: Requires STATSIG_CONSOLE_API_KEY.

Read a specific feature gate
- **get_layer**: Requires STATSIG_SERVER_SECRET_KEY.

Fetches parameter values from a layer
- **list_dynamic_configs**: Requires STATSIG_CONSOLE_API_KEY.

List all dynamic configs in the project
- **list_gates**: Requires STATSIG_CONSOLE_API_KEY.

List all feature gates in the project
- **log_event**: Requires STATSIG_SERVER_SECRET_KEY.

Logs custom events for analytics and metric calculation
- **update_gate**: Requires STATSIG_CONSOLE_API_KEY.

Update an existing feature gate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Statsig** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the gate 'new_checkout_flow' is enabled for user 'user_99'."

**🤖 AI Agent:**
> I've checked the gate 'new_checkout_flow' for user 'user_99'. The gate is currently **Open** (True).

---

**👤 You:**
> "List all feature gates in my Statsig project."

**🤖 AI Agent:**
> I've retrieved the list of gates. You have 3 active gates: 'ai_beta_access', 'dark_mode_v2', and 'new_checkout_flow'.

---

**👤 You:**
> "Create a new feature gate named 'mobile_redesign' with description 'Testing new UI'."

**🤖 AI Agent:**
> The feature gate 'mobile_redesign' has been successfully created in your project.


## ❓ FAQ

**Q: What is the difference between the Server Secret Key and the Console API Key?**
The Server Secret Key is used for evaluation tools like `check_gate` and `get_config`. The Console API Key is required for management actions like `list_gates` or `create_gate`.

**Q: How do I evaluate a gate for a specific user?**
Use the `check_gate` tool. You must provide the `gateName` and a `user` JSON object containing at least a `userID` (e.g., `{"userID": "123"}`).

**Q: Can I log custom events for analytics?**
Yes, use the `log_event` tool to send an array of event objects including name, value, and user metadata to Statsig for real-time metric calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statsig](https://vinkius.com/mcp/statsig)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Statsig** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `statsig` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Statsig** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "statsig": {
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
