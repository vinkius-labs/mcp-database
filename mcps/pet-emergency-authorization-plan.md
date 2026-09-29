# Pet Emergency Authorization Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-emergency-authorization-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Manage pet emergency contacts, caregiver permissions, and medical access protocols.

## Description
This MCP server provides a structured framework for managing pet emergency protocols. It allows AI agents to retrieve critical information including `get_emergency_contact_card` for immediate veterinary needs, `get_caregiver_authorization_record` to verify legal permissions, and `get_communication_sequence` to follow strict notification hierarchies. It also facilitates document retrieval via `get_document_access_instructions` and ensures plan validity through `get_annual_review_checklist`.


## Available Tools (5)
- **get_annual_review_checklist**: Generates a structured list of items that must be audited to ensure the plan's validity
- **get_caregiver_authorization_record**: Retrieves the specific legal and medical permissions granted to a designated caregiver
- **get_communication_sequence**: Provides the exact step-by-step notification list to be followed during an incident
- **get_document_access_instructions**: Retrieves the necessary guidance for providers to access insurance information and medical records
- **get_emergency_contact_card**: Generates a concise, high-level summary for immediate presentation to a veterinary provider during an emergency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Emergency Authorization Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an emergency contact card for my dog, Buddy."

**🤖 AI Agent:**
> Pet Name: Buddy. Owner: Alex Smith. Primary Contact: Jordan Lee (555-0123).

---

**👤 You:**
> "What is the notification sequence for a medical emergency?"

**🤖 AI Agent:**
> 1. Primary Contact: Jordan Lee (Phone). 2. Secondary Contact: Sam Rivera (Email).

---

**👤 You:**
> "What are the instructions for a veterinary provider to access insurance?"

**🤖 AI Agent:**
> Please present the policy number 98765-ABC and the digital authorization form found in the pet's medical folder.


## ❓ FAQ

**Q: How can I see the primary contact for my pet?**
You can use the `get_emergency_contact_card` tool to generate a summary containing the primary contact's name and phone number.

**Q: Can I check if a caregiver has medical authority?**
Yes, the `get_caregiver_authorization_record` tool retrieves the specific medical scope and decisions authorized for a designated person.

**Q: How do I know who to call first during a medical incident?**
Use the `get_communication_sequence` tool with the incident type 'medical' to see the exact notification order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-emergency-authorization-plan](https://vinkius.com/en/ai-agent-connect/pet-emergency-authorization-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Emergency Authorization Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-emergency-authorization-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Emergency Authorization Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-emergency-authorization-plan": {
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
