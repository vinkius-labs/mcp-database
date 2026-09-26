# Family Contact Tree MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-contact-tree)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Manage hierarchical family contact structures and calculate prioritized notification sequences.

## Description
This MCP server provides tools to manage complex family contact hierarchies. It allows for retrieving specific contact details using `get_contact_details`, validating the logical integrity of the family tree with `validate_relationship_integrity`, generating prioritized call sequences via `calculate_notification_sequence`, and visualizing the structure through `get_family_hierarchy`.


## Available Tools (4)
- **calculate_notification_sequence**: Generates the ordered list of contact attempts based on the provided notification priority
- **get_contact_details**: Retrieves the specific profile and role information for a single individual
- **get_family_hierarchy**: Returns a view of the family tree organized by levels
- **validate_relationship_integrity**: Ensures that all defined relationships in the tree are valid and do not create impossible loops or orphaned nodes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Contact Tree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the hierarchy starting from John Doe."

**🤖 AI Agent:**
> The family hierarchy for John Doe includes his spouse Jane Doe and children Alice and Bob.

---

**👤 You:**
> "What is the notification sequence for the order: Alice, Bob, Jane?"

**🤖 AI Agent:**
> The contact sequence is: 1. Alice, 2. Bob, 3. Jane.

---

**👤 You:**
> "Get the details for contact 'Mary Smith'."

**🤖 AI Agent:**
> Mary Smith is a Backup contact and is currently active in the tree.


## ❓ FAQ

**Q: How can I see the full structure of my family tree?**
You can use the `get_family_hierarchy` tool to receive a nested view of the tree starting from a specific root contact.

**Q: What happens if a preferred contact is unavailable?**
The `calculate_notification_sequence` tool generates a prioritized list of contact attempts based on your specified notification order, ensuring backup contacts are reached in the correct sequence.

**Q: How do I ensure my family tree has no errors?**
Use the `validate_relationship_integrity` tool to check for impossible loops or orphaned nodes within your tree structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-contact-tree](https://vinkius.com/en/ai-agent-connect/family-contact-tree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Contact Tree** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-contact-tree` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Contact Tree** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-contact-tree": {
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
