# Document Collection Appointment Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/document-collection-appointment-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured appointment briefs and actionable checklists for document collection logistics.

## Description
This MCP server provides a suite of tools to manage document retrieval logistics. Use `generate_appointment_brief` to create a formal summary of meeting details, including locations and security requirements. Use `generate_checklist` to produce a dual-category 'Bring and Complete' list for users. You can also use `validate_collection_readiness` to check if all necessary items are present, or `format_location_guide` to provide specific venue instructions.


## Available Tools (4)
- **format_location_guide**: Provides detailed context or instructions regarding the collection venue
- **generate_appointment_brief**: Generates a comprehensive formal summary of all appointment details
- **generate_checklist**: Transforms a complete appointment briefing into a dual-category checklist (Bring vs. Complete)
- **validate_collection_readiness**: Answers "Am I ready for my appointment?" by checking a user's current state against the requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Document Collection Appointment Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an appointment brief for collecting a passport at the City Hall on October 12th at 10:00 AM. Documents: Passport, Birth Certificate. Required ID: Driver's License. Collector: John Doe. Steps: Show ID, sign log, receive receipt."

**🤖 AI Agent:**
> Appointment Brief: Passport collection at City Hall on October 12th, 10:00 AM. You must present your Driver's License to John Doe. Required documents: Passport, Birth Certificate. Steps: 1. Show ID, 2. Sign log, 3. Receive receipt.

---

**👤 You:**
> "Create a checklist from this brief: { "briefSummary": "Legal Doc Pickup", "documentList": ["Contract"], "requiredId": ["ID Card"], "confirmationSteps": ["Sign document"] }"

**🤖 AI Agent:**
> Bring: Contract, ID Card. Complete: Sign document.

---

**👤 You:**
> "Am I ready for my appointment? I have: ['Contract', 'ID Card']. Brief: { "documentList": ["Contract"], "requiredId": ["ID Card"] }"

**🤖 AI Agent:**
> Yes, you are ready for your appointment.


## ❓ FAQ

**Q: How do I create a checklist for my appointment?**
First, use `generate_appointment_brief` to create the formal summary. Then, pass that summary into `generate_checklist` to get your 'Bring' and 'Complete' lists.

**Q: Can I check if I have all my documents ready?**
Yes, use the `validate_collection_readiness` tool by providing the items you currently have and the original appointment brief.

**Q: What information is needed for the appointment brief?**
You need to provide the document list, the collection location, the appointment date, required identification, the authorized collector, and the confirmation steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/document-collection-appointment-brief](https://vinkius.com/en/ai-agent-connect/document-collection-appointment-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Document Collection Appointment Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `document-collection-appointment-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Document Collection Appointment Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "document-collection-appointment-brief": {
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
