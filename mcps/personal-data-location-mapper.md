# Personal Data Location Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-data-location-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Map and audit the physical and digital locations of your personal data.

## Description
This MCP server provides a specialized toolset for mapping, auditing, and querying the locations of personal data across devices, cloud services, and physical storage. Use `get_data_category_locations` to find where specific information like Financial or Identity data is stored, or use `find_location_details` to check the custodian and backup status of a specific device or folder. It also includes `audit_custodian_exposure` to review what data a specific entity manages and `verify_backup_integrity` to ensure your critical data categories have valid redundant copies.


## Available Tools (4)
- **find_location_details**: Get details about a specific data location
- **get_data_category_locations**: Find all locations associated with a specific data category
- **verify_backup_integrity**: Verify if a data category is safely backed up
- **audit_custodian_exposure**: Audit the data inventory managed by a custodian


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Data Location Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is my Identity data located?"

**🤖 AI Agent:**
> Your Identity data is located in your Passport (Physical Safe Box) and your Birth Certificate (iCloud).

---

**👤 You:**
> "What is the backup status for my Work Laptop?"

**🤖 AI Agent:**
> The Work Laptop is managed by you, and its data is backed up to your Google Drive.

---

**👤 You:**
> "Is my Health data safely backed up?"

**🤖 AI Agent:**
> Yes, your Health data is covered with backups available in your Dropbox account.


## ❓ FAQ

**Q: How can I find where my financial records are stored?**
You can use the `get_data_category_locations` tool and specify 'Financial' as the data category to see all associated locations.

**Q: Can I check if my data is properly backed up?**
Yes, the `verify_backup_integrity` tool allows you to check the backup coverage for any specific data category.

**Q: How do I see what data a specific service provider manages?**
Use the `audit_custodian_exposure` tool by providing the name of the service provider or person acting as the custodian.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-data-location-mapper](https://vinkius.com/en/ai-agent-connect/personal-data-location-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Data Location Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-data-location-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Data Location Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-data-location-mapper": {
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
