# Emergency Medication Records Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-medication-records-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Securely organize medication data, contact lists, and compliance checklists for emergency preparedness.

## Description
This MCP server provides a secure bridge for AI agents to manage critical medication information. It enables users to process medication entries using `analyze_medication_entry` to ensure strict adherence to label-only data rules. The server can generate high-level summaries for responders via `generate_emergency_records_card`, create upcoming action schedules with `generate_reminder_calendar`, manage authorized access through `compile_authorized_contact_list`, and provide synchronization guides with `generate_document_update_checklist`.


## Available Tools (5)
- **generate_emergency_records_card**: Produce a concise, high-level summary for emergency responders
- **generate_reminder_calendar**: Create a schedule of upcoming medication actions
- **analyze_medication_entry**: Process raw medication data and validate it against domain rules
- **compile_authorized_contact_list**: Manage and list the individuals authorized to access the records
- **generate_document_update_checklist**: Provide a step-by-step guide for synchronizing digital records with physical inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Medication Records Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a new medication: Aspirin, prescribed by Dr. Smith, last refilled on 2023-10-01, storage is 'Store in a cool, dry place', expires 2025-12-31. Please validate this entry."

**🤖 AI Agent:**
> The medication entry for Aspirin is Compliant. It follows the Label-Only rule and no expiry alerts are active.

---

**👤 You:**
> "Generate a summary for my emergency contact, Jane Doe, who has Full access."

**🤖 AI Agent:**
> Your emergency records card has been generated. It includes medication summaries for Aspirin and Ibuprofen with the access code: 8829-XJ.

---

**👤 You:**
> "My physical inventory shows that some items are expired. What should I do?"

**🤖 AI Agent:**
> Please follow these steps: 1. Remove all expired medications from your physical supply. 2. Update the digital records to reflect the removal. 3. Check the `expiryAlert` status for remaining items.


## ❓ FAQ

**Q: How does the system ensure data accuracy?**
The system uses `analyze_medication_entry` to enforce a 'Label-Only' rule, ensuring that only information explicitly stated on the medication label is recorded, preventing unverified medical advice.

**Q: Can I share my records with emergency responders?**
Yes. You can use `generate_emergency_records_card` to create a concise summary containing only essential safety information and an access code for authorized individuals.

**Q: How are expiration dates managed?**
The `generate_reminder_calendar` tool tracks expiration dates and generates alerts based on a user-defined notification lead time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-medication-records-plan](https://vinkius.com/en/ai-agent-connect/emergency-medication-records-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Medication Records Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-medication-records-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Medication Records Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-medication-records-plan": {
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
