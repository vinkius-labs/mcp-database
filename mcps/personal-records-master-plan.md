# Personal Records Master Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-records-master-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic engine to transform document inventories into structured records architectures.

## Description
This MCP server provides a suite of tools to organize household and personal documentation. It applies a fixed taxonomy to categorize records, enforces least-access security protocols, and generates migration sequences, responsibility maps, and annual review calendars. Use `get_records_architecture` to build your blueprint, `plan_migration_sequence` to organize movement, `generate_responsibility_map` to assign roles, and `create_review_calendar` to schedule audits.


## Available Tools (4)
- **create_review_calendar**: 
- **generate_responsibility_map**: 
- **get_records_architecture**: 
- **plan_migration_sequence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Records Master Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me organize my documents. I have identity papers, tax returns, and medical records. I want to store them in a digital vault and a physical safe."

**🤖 AI Agent:**
> I have generated your records architecture. Identity papers are assigned to the Physical Safe (Isolated), Tax returns to the Digital Vault (Protected), and Medical records to the Digital Vault (Protected).

---

**👤 You:**
> "Who should have access to our house deed and utility bills?"

**🤖 AI Agent:**
> Based on your access needs, the House Deed is assigned to the Head of Household as a Custodian, while utility bills are accessible to all adult members as Viewers.

---

**👤 You:**
> "When should I review my financial records?"

**🤖 AI Agent:**
> Your annual review for Financial records is scheduled for April 15th, following your preferred retention logic.


## ❓ FAQ

**Q: How does the tool handle sensitive documents?**
The server uses a strict security protocol that pairs high-sensitivity categories with high-security storage locations, such as isolated or protected vaults.

**Q: Can I assign different roles to household members?**
Yes, using `generate_responsibility_map`, you can define specific Custodians and Viewers based on the principle of least-access.

**Q: What is the purpose of the review calendar?**
The `create_review_calendar` tool produces a yearly schedule to ensure sensitive records are audited and outdated documents are purged according to retention rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-records-master-plan](https://vinkius.com/en/ai-agent-connect/personal-records-master-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Records Master Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-records-master-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Records Master Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-records-master-plan": {
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
