# Crop Share Lease Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crop-share-lease-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Models and compares crop-share lease arrangements against cash rent.

## Description
This MCP server provides specialized financial modeling for agricultural lease agreements. It allows users to calculate the exact revenue and net returns for both landlords and tenants using `calculate_crop_share_splits`. Users can retrieve industry-standard configurations like 50/50 or 60/40 splits via `get_standard_models`, and perform risk-reward analysis by using `compare_lease_types` to evaluate crop-share models against traditional cash rent scenarios.


## Available Tools (3)
- **get_standard_models**: 
- **calculate_crop_share_splits**: 
- **compare_lease_types**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crop Share Lease Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the splits for a 50/50 crop share with $100,000 revenue, $20,000 seed, $10,000 fertilizer, $5,000 chemicals, and $5,000 harvest costs."

**🤖 AI Agent:**
> The landlord's net return is $30,000 and the tenant's net return is $30,000.

---

**👤 You:**
> "What are the revenue and cost shares for a 60/40 model?"

**🤖 AI Agent:**
> In a 60/40 model, the landlord receives 60% of the revenue and bears 60% of the costs.

---

**👤 You:**
> "Is a crop share with $40,000 landlord net return better than a $35,000 cash rent?"

**🤖 AI Agent:**
> Yes, the Crop Share model is preferred for the landlord as it results in a higher net return.


## ❓ FAQ

**Q: How do I calculate the net return for a landlord?**
You can use the `calculate_crop_share_splits` tool. It takes total revenue, input costs, and the landlord's revenue and cost shares to return the final net profit.

**Q: Can I compare a crop-share lease to a cash rent lease?**
Yes, the `compare_lease_types` tool is designed specifically to compare the net returns of a crop-share arrangement against a fixed cash rent amount.

**Q: What are the standard lease models available?**
The `get_standard_models` tool provides predefined splits for common models including 50/50, 60/40, and the 2/3-1/3 model.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crop-share-lease-calculator](https://vinkius.com/ai-agent-connect/crop-share-lease-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crop Share Lease Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crop-share-lease-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crop Share Lease Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crop-share-lease-calculator": {
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
