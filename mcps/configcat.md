# ConfigCat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/configcat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage feature flags and remote configurations via ConfigCat — list environments, create settings, and toggle features directly from your AI agent.

## Description
Connect **ConfigCat** to any AI agent to streamline your feature flag management and release workflows through natural conversation.

### What you can do

- **Configurations & Environments** — List, create, and manage configuration containers and environments (Test, Staging, Production) across your products.
- **Feature Flags & Settings** — Create and inspect feature flags or settings (boolean, string, int, double) to control application logic.
- **Value Management** — Retrieve and update setting values dynamically to trigger real-time changes in your software without redeploying.
- **Segment Control** — Manage user segments to target specific groups for canary releases or A/B testing.

### How it works

1. Subscribe to this server
2. Enter your ConfigCat API Key ID and Secret
3. Start managing your feature toggles from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — toggle features and check flag statuses directly from the code editor to maintain focus.
- **DevOps Engineers** — manage environments and configurations as part of the CI/CD workflow via automated agents.
- **Product Managers** — oversee feature rollouts and user segments through simple chat commands without technical overhead.


## Available Tools
- **create_config**: Create a new configuration
- **create_environment**: Create a new environment
- **create_segment**: Create a new segment
- **create_setting**: Create a new feature flag or setting
- **delete_config**: Delete a configuration
- **delete_environment**: Delete an environment
- **delete_segment**: Delete a segment
- **delete_setting**: Delete a setting
- **get_config**: Get details of a specific configuration
- **get_environment**: Get details of an environment
- **get_segment**: Get details of a segment
- **get_setting**: Get details of a setting
- **get_setting_value**: Get the value of a setting in an environment
- **list_configs**: List all configurations in a product
- **list_environments**: g., Test, Production) for a specific product.

List all environments in a product
- **list_segments**: List all segments in a product
- **list_settings**: List all settings in a configuration
- **update_setting_value**: Update the value/targeting of a setting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ConfigCat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all configurations for product ID 'prod_123'."

**🤖 AI Agent:**
> I've found 2 configurations for product 'prod_123': 'Main App Config' (ID: conf_abc) and 'Mobile API Config' (ID: conf_xyz).

---

**👤 You:**
> "Create a new boolean feature flag called 'Beta Feature' in config 'conf_abc'."

**🤖 AI Agent:**
> Successfully created the boolean feature flag 'Beta Feature' (key: betaFeature) in configuration 'conf_abc'.

---

**👤 You:**
> "Show me the details for environment 'env_987'."

**🤖 AI Agent:**
> Environment 'env_987' is named 'Production'. It is associated with Product ID 'prod_123' and has the color code '#FF0000'.


## ❓ FAQ

**Q: Can I list all feature flags in a specific configuration?**
Yes. Use the `list_settings` tool with your Configuration ID to retrieve all feature flags and settings, including their types and keys.

**Q: How do I create a new environment like 'Staging'?**
Simply use the `create_environment` tool. Provide the Product ID and the name 'Staging' to instantly set up a new environment for your flags.

**Q: Is it possible to update the value of a setting remotely?**
Yes! The `update_setting_value` tool allows you to change the value of any flag or setting for a specific environment in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/configcat](https://vinkius.com/mcp/configcat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ConfigCat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `configcat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ConfigCat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "configcat": {
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
