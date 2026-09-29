# Personal Assets Record Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-assets-record-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage high-value assets with evidence linking and insurance-ready reporting.

## Description
This MCP server provides a structured system for tracking high-value personal property. It enables users to register assets with sensitivity tiers, link digital evidence like receipts and photos, and manage annual verification tasks to maintain insurance readiness. Use `register_asset_entry` to add new items, `get_asset_registry` to filter your collection, and `generate_insurance_summary` to create professional reports for adjusters. It also supports archiving records via `archive_asset_record` to preserve history for sold or lost items.


## Available Tools (5)
- **archive_asset_record**: Move an asset to a secure, read-only archive
- **create_verification_task**: Generate a task to fulfill the annual verification requirement
- **generate_insurance_summary**: Compile a professional, read-only report for insurance adjusters
- **get_asset_registry**: You can filter by sensitivity tier, verification status, or insurance readiness.

Retrieve a complete list of assets filtered by specific criteria
- **register_asset_entry**: Ensure purchase details are provided.

Create a new asset record within the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Assets Record Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register a new Rolex watch located in the home safe costing $10,000 purchased on 2023-05-15 from Rolex Boutique."

**🤖 AI Agent:**
> The Rolex watch has been successfully registered with a Confidential tier and is currently unverified.

---

**👤 You:**
> "Show me all my verified assets."

**🤖 AI Agent:**
> I found 3 verified assets in your registry: Rolex Watch, Diamond Ring, and Vintage Camera.

---

**👤 You:**
> "Generate an insurance report for my confidential items including maintenance history."

**🤖 AI Agent:**
> The insurance summary report has been generated, including maintenance history for your high-value confidential assets.


## ❓ FAQ

**Q: How do I ensure my assets are insurance-ready?**
An asset is insurance-ready when it has linked evidence (like a receipt) and a valid valuation. You can use `generate_insurance_summary` to view all assets that meet these criteria.

**Q: What are sensitivity tiers?**
Tiers (Public, Private, Confidential) determine how much information is exposed. Confidential items require higher protection for sensitive details like serial numbers.

**Q: Can I recover an archived asset?**
Archived assets are moved to a secure, read-only state to preserve historical records. They cannot be modified through standard registration tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-assets-record-plan](https://vinkius.com/en/ai-agent-connect/personal-assets-record-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Assets Record Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-assets-record-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Assets Record Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-assets-record-plan": {
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
