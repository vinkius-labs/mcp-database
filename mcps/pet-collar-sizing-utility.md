# Pet Collar Sizing Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-collar-sizing-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Verify pet collar fit and explore available sizing tiers.

## Description
This MCP server provides tools to ensure your pet's comfort by matching neck measurements to collar sizes. Use `get_collar_sizes` to browse the catalog, `check_fit_compatibility` to verify a specific collar, `find_best_fitting_collars` to discover suitable options, or `summarize_tier_availability` to see the coverage of a specific size tier.


## Available Tools (4)
- **find_best_fitting_collars**: Find all collars that fit a specific neck measurement
- **get_collar_sizes**: Get available collar sizes from the catalog
- **summarize_tier_availability**: Summarize the sizing coverage for a specific tier
- **check_fit_compatibility**: Check if a specific collar fits a pet neck measurement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Collar Sizing Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What collars are available in the Small tier?"

**🤖 AI Agent:**
> The Small tier includes the Puppy Comfort Collar and the Tiny Tail Guard.

---

**👤 You:**
> "Will a collar with ID 'collar-123' fit a pet with a 15cm neck?"

**🤖 AI Agent:**
> Yes, the collar-123 is a Perfect Fit for a 15cm neck measurement.

---

**👤 You:**
> "Find me collars that fit a 25cm neck measurement."

**🤖 AI Agent:**
> The following collars fit a 25cm neck: Standard Fit Pro (Tier: Standard) and Active Pet Collar (Tier: Standard).


## ❓ FAQ

**Q: How do I know if a collar will fit my pet?**
You can use the `find_best_fitting_collars` tool by providing your pet's neck measurement to see all compatible options.

**Q: Can I filter collars by size category?**
Yes, the `get_collar_sizes` tool allows you to filter the catalog by specific tiers like Small, Medium, or Large.

**Q: What information is provided for a specific collar fit?**
Using `check_fit_compatibility` will return the collar name, whether it is compatible, and a fit status description.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-collar-sizing-utility](https://vinkius.com/en/ai-agent-connect/pet-collar-sizing-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Collar Sizing Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-collar-sizing-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Collar Sizing Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-collar-sizing-utility": {
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
