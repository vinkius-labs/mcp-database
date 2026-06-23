# Litter Size Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/litter-size-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [biology](../categories/biology.md)

Predict puppy litter sizes based on breed and physical size.

## Description
The Litter Size Estimator provides biological predictions for canine litters. By using the `calculate_litter_estimate` tool, you can input a specific breed and size (Small, Medium, or Large) to retrieve the estimated minimum, maximum, and average number of puppies. You can also use `lookup_breed_statistics` to see general trends for a breed or `list_supported_degrees` to see all available breeds in the database.


## Available Tools (3)
- **calculate_litter_estimate**: Predict the number of puppies based on breed and size
- **list_supported_breeds**: List all supported breeds
- **lookup_breed_statistics**: Get general litter size statistics for a breed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Litter Size Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected litter size for a Golden Retriever that is Medium sized?"

**🤖 AI Agent:**
> For a Medium-sized Golden Retriever, the estimated average litter size is 6 puppies (Range: 4 - 8).

---

**👤 You:**
> "Show me all breeds available in the estimator."

**🤖 AI Agent:**
> The following breeds are supported: [List of breeds retrieved via `list_supported_breeds`].

---

**👤 You:**
> "What are the general statistics for a Bulldog?"

**🤖 AI Agent:**
> The general litter size statistics for a Bulldog are: Average 5, Minimum 3, Maximum 7.


## ❓ FAQ

**Q: How accurate are these estimates?**
Estimates are based on hardcoded population datasets representing biological trends in specific breeds and size classes.

**Q: What dog sizes are supported?**
The tool supports three physical categories: Small, Medium, and Large.

**Q: Can I see all available breeds?**
Yes, you can use the `list_supported_breeds` tool to retrieve a complete list of all supported breed names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/litter-size-estimator](https://vinkius.com/mcp/litter-size-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Litter Size Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `litter-size-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Litter Size Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "litter-size-estimator": {
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
