# Insurance Document Retention Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insurance-document-retention-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Automated storage and review scheduling for insurance documentation.

## Description
This MCP server provides tools to manage the lifecycle of insurance documents. It allows AI agents to retrieve retention rules via `get_retention_schedule`, calculate specific document disposition dates with `calculate_document_disposition`, generate comprehensive storage plans using `generate_storage_plan`, and identify regulatory risks through `evaluate_compliance_risk`. It ensures compliance by mapping document types to required storage tiers like Hot, Cold, or Ready for Purge.


## Available Tools (4)
- **calculate_document_disposition**: Determine when a specific document is due for review or destruction
- **evaluate_compliance_risk**: Identify compliance risks in a storage plan
- **generate_storage_plan**: Create a comprehensive storage and review plan for a policy
- **get_retention_schedule**: Retrieve standard retention rules for a document type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insurance Document Retention Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a storage plan for policy ID POL-998 with these claim dates: 2023-01-15 and 2023-06-20, and renewal dates: 2024-01-01."

**🤖 AI Agent:**
> The storage plan for policy POL-998 includes 2 claims in Hot storage and the renewal record in Hot storage, with a review scheduled for 2025-01-01.

---

**👤 You:**
> "What is the retention rule for a 'claim' document type?"

**🤖 AI Agent:**
> Claims must be retained for 7 years from the trigger date according to the Standard regulatory tier.

---

**👤 You:**
> "Check if there are any compliance risks for this storage plan: {"documents": [{"documentId": "DOC-1", "storageTier": "Ready for Purge", "reviewDate": "2023-01-01"}]} under the 'Standard' tier."

**🤖 AI Agent:**
> No high-level compliance risks were identified for the provided storage plan under the Standard tier.


## ❓ FAQ

**Q: How does the retention period get calculated?**
The retention period is determined by the intersection of the document type and the regulatory tier, or by a user-provided override via `calculate_document_disposition`.

**Q: What are the different storage tiers?**
Documents are assigned to Hot storage if active, Cold storage if nearing their end date, or marked Ready for Purge if they have passed their retention date.

**Q: Can I override standard retention rules?**
Yes, you can use the `calculate_document_disposition` tool with the `userOverrideYears` parameter to extend the retention of a specific document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insurance-document-retention-plan](https://vinkius.com/en/ai-agent-connect/insurance-document-retention-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insurance Document Retention Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insurance-document-retention-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insurance Document Retention Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insurance-document-retention-plan": {
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
