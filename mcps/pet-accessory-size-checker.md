# Pet Accessory Size Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-accessory-size-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Verify if pet measurements fit specific accessory sizes.

## Description
This MCP server provides tools to ensure pet accessories like collars and harnesses fit perfectly. Use `check_accessory_fit` to compare a measurement against a size range, `list_accessory_sizes` to see available options, `get_size_range_details` for specific bounds, and `validate_measurement_type` to confirm if a dimension is supported for a category.


## Available Tools (4)
- **check_accessory_fit**: Determines if a specific pet measurement fits a given accessory size
- **get_size_range_details**: Provides the specific minimum and maximum measurement bounds for a specific accessory size
- **list_accessory_sizes**: Retrieves all available sizes for a specific category of accessory
- **validate_measurement_type**: Verifies if a specific measurement type is relevant and supported for a given accessory category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Accessory Size Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will a small collar fit my pet with a 15cm neck circumference?"

**🤖 AI Agent:**
> Yes, the measurement fits within the specified range.

---

**👤 You:**
> "Is a 25cm chest girth too large for a medium harness?"

**🤖 AI Agent:**
> No, the measurement is too large for the medium size.

---

**👤 You:**
> "What sizes are available for the harness category?"

**🤖 AI Agent:**
> The available sizes for harnesses are small, medium, and large.


## ❓ FAQ

**Q: How do I know if a collar will fit my dog?**
You can use the `check_accessory_fit` tool by providing the collar category ID, the size ID, and your dog's neck measurement.

**Q: What measurement types are supported?**
Supported types vary by category. You can use `validate_measurement_type` to see which dimensions, such as neck circumference or chest girth, are valid for a specific accessory.

**Q: Can I see the exact measurement ranges for a size?**
Yes, use `get_size_range_details` to retrieve the minimum and maximum bounds for any specific size and measurement type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-accessory-size-checker](https://vinkius.com/en/ai-agent-connect/pet-accessory-size-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Accessory Size Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-accessory-size-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Accessory Size Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-accessory-size-checker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
