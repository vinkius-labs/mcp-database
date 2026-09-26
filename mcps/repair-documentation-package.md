# Repair Documentation Package MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-documentation-package)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Standardize repair evidence into a structured, searchable project record.

## Description
This MCP server provides a specialized document organization and lifecycle management system. It applies a fixed folder taxonomy and strict filename patterns to transform disparate repair evidence--such as invoices, photos, and permits--into a structured, searchable project record. Use `get_organized_record_plan` to view the document hierarchy, `generate_capture_checklist` to identify missing evidence, `create_handoff_summary` for contractor handoffs, and `validate_document_upload` to ensure all files meet project standards.


## Available Tools (4)
- **validate_document_upload**: 
- **create_handoff_summary**: 
- **generate_capture_checklist**: 
- **get_organized_record_plan**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Documentation Package** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the organized folder structure for project PROJ-123."

**🤖 AI Agent:**
> The project PROJ-123 is organized into the following hierarchy: /Financial, /Administrative, /Visual, and /Technical.

---

**👤 You:**
> "What documents are missing for the Electrical repair in project ELEC-456?"

**🤖 AI Agent:**
> The record for ELEC-456 is currently Partial. The following mandatory documents are missing: Permit_01.pdf and Invoice_99.pdf.

---

**👤 You:**
> "Is the filename 'REP-789_Invoice_20231012_Plumbing.pdf' valid for project REP-789?"

**🤖 AI Agent:**
> Yes, the filename is valid and follows the required taxonomy for project REP-789.


## ❓ FAQ

**Q: How do I check if my repair record is complete?**
You can use the `generate_capture_checklist` tool. It compares your current documents against the required tier for your specific repair type and lists any missing items.

**Q: How can I ensure my filenames are correct?**
Use the `validate_document_upload` tool. It checks if your filename follows the mandatory [ProjectID]_[DocType]_[YYYYMMDD]_[Description] pattern and suggests corrections if needed.

**Q: What information is included in the handoff summary?**
The `create_handoff_summary` tool synthesizes completion notes, contractor contacts, and invoices into a narrative overview, including key contacts and critical maintenance alerts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-documentation-package](https://vinkius.com/en/ai-agent-connect/repair-documentation-package)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Documentation Package** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-documentation-package` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Documentation Package** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-documentation-package": {
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
