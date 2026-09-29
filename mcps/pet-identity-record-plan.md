# Pet Identity Record Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-identity-record-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [management](../categories/management.md)

Manage pet identification, ownership, and privacy boundaries with structured record packets.

## Description
This MCP server provides a structured management system for organizing pet identification, ownership, and medical/legal records. It allows owners to enforce privacy boundaries by defining which specific data fields are visible to different tiers of contacts. Use `generate_records_packet` to create filtered snapshots for veterinarians or sitters, `manage_access_list` to control authorized access, `create_recovery_sheet` for emergency contact info, and `schedule_review_cycle` to maintain accurate records. It connects your pet's identity data to AI agents via Vinkius Edge.


## Available Tools (4)
- **create_recovery_sheet**: Generates a simplified contact sheet for emergency situations
- **generate_records_packet**: Creates a filtered snapshot of pet information tailored for a specific recipient
- **manage_access_list**: Updates the list of individuals authorized to view pet records
- **schedule_review_cycle**: Sets up a recurring reminder to audit records and access permissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Identity Record Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a record packet for my dog Buddy for a sitter."

**🤖 AI Agent:**
> The record packet for Buddy has been generated for the sitter role, containing only the permitted identity and contact details.

---

**👤 You:**
> "Add Sarah to the access list for pet ID 123 with limited access."

**🤖 AI Agent:**
> Sarah has been added to the authorized access list for pet ID 123 with limited access level.

---

**👤 You:**
> "Create an emergency recovery sheet for my cat Luna."

**🤖 AI Agent:**
> The emergency recovery sheet for Luna has been created, containing the primary owner's contact and designated recovery contacts.


## ❓ FAQ

**Q: How do I share pet info with a veterinarian?**
You can use the `generate_records_packet` tool to create a filtered snapshot of the pet's information specifically for a veterinarian role.

**Q: Can I remove someone from the authorized list?**
Yes, you can use `manage_access_list` with the removal flag to update your authorized access list.

**Q: What happens in an emergency?**
You can use `create_recovery_sheet` to generate a simplified contact sheet that contains only essential contact information for emergency situations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-identity-record-plan](https://vinkius.com/en/ai-agent-connect/pet-identity-record-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Identity Record Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-identity-record-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Identity Record Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-identity-record-plan": {
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
