# Legacy Blog Preservation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/legacy-blog-preservation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Generates actionable preservation checklists for digital assets and legacy websites.

## Description
This MCP server provides a suite of tools for digital archivists to manage the lifecycle of legacy web content. Use `get_preservation_plan` to generate structured checklists based on site URLs and maintenance instructions. You can also use `validate_asset_integrity` to verify file counts, `calculate_preservation_timeline` to map out project milestones, and `verify_destination_readiness` to ensure target storage has sufficient capacity.


## Available Tools (4)
- **get_preservation_plan**: Generates a structured, executable checklist based on provided preservation variables
- **validate_asset_integrity**: Checks if the provided media folders and archives match the expected content list
- **verify_destination_readiness**: Confirms that the target backup destinations are available and have sufficient capacity
- **calculate_preservation_timeline**: Determines the urgency and milestone dates for the preservation project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legacy Blog Preservation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a preservation plan for https://oldblog.com using archives at /data/archives and media at /data/media, with a target date of 2025-12-31 and instructions to migrate the site."

**🤖 AI Agent:**
> 1. Verify integrity of media at /data/media. 2. Extract content from /data/archives. 3. Migrate site content to the new platform. 4. Verify successful migration by checking target URL.

---

**👤 You:**
> "Calculate the timeline for a preservation project starting today and ending on 2024-06-01."

**🤖 AI Agent:**
> The project has 120 days remaining. Milestones: Inventory phase ends on 2024-03-15, Execution phase ends on 2024-05-01, and Verification phase ends on 2024-06-01.

---

**👤 You:**
> "Check if the destination /mnt/archive/ has enough space for 50GB of data."

**🤖 AI Agent:**
> The destination /mnt/archive/ is ready. It has 120GB of available space, which is sufficient for the 50GB requirement.


## ❓ FAQ

**Q: How do I generate a preservation checklist?**
Provide the site URLs, media folders, and maintenance instructions to the `get_preservation_plan` tool to receive an ordered list of tasks.

**Q: Can I verify if my backup storage is ready?**
Yes, use the `verify_destination_readiness` tool by providing the target paths and the estimated size of the assets in GB.

**Q: How can I check if all files were successfully moved?**
Use the `validate_asset_integrity` tool to compare the actual file count in your destination against the expected count from your inventory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/legacy-blog-preservation-plan](https://vinkius.com/en/ai-agent-connect/legacy-blog-preservation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legacy Blog Preservation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legacy-blog-preservation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legacy Blog Preservation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legacy-blog-preservation-plan": {
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
