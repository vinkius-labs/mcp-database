# Care Communication & Consent Map MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-communication-consent-map)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

A privacy-first decision engine for managing communication permissions and data disclosure boundaries.

## Description
This MCP server provides a privacy-first decision engine designed to manage the complex intersection of healthcare privacy and relational transparency. It applies least-disclosure rules and explicit consent precedence to determine exactly what information can be shared with whom. Using tools like `query_communication_matrix` to map permissions, `get_update_templates` for role-based messaging, `check_restriction_flags` to identify privacy barriers, and `calculate_review_schedule` for compliance monitoring, it ensures all communications remain within legal and ethical boundaries.


## Available Tools (4)
- **calculate_review_schedule**: Calculates the next required review schedule
- **check_restriction_flags**: Checks if communication is restricted based on subject and recipient
- **get_update_templates**: Generates approved text templates for communicating specific information
- **query_communication_matrix**: Determines exactly what can be communicated to whom and via which methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Communication & Consent Map** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is allowed to receive medical information for patient ID 123?"

**🤖 AI Agent:**
> Based on current consents, the following individuals are allowed to receive medical information: Legal Guardian (ID: 456) and Primary Caregiver (ID: 789).

---

**👤 You:**
> "Generate a message for the Primary Caregiver about the patient's recent checkup."

**🤖 AI Agent:**
> Dear Primary Caregiver, this is an update regarding the patient's recent checkup. The results indicate that all vitals are within normal ranges.

---

**👤 You:**
> "Is the neighbor allowed to receive emergency contact details?"

**🤖 AI Agent:**
> No, the neighbor (ID: 001) does not have permission to receive emergency contact details under the current consent configuration.


## ❓ FAQ

**Q: How does the system handle conflicting permissions?**
The system follows the Explicit Consent Precedence rule: if a person has explicitly denied permission for a specific category, that denial overrides any general permission.

**Q: What is the 'Least-Disclosure Rule'?**
In the absence of explicit permission, the system defaults to the most restrictive state. Information is only shared if there is a clear, valid permission associated with the recipient.

**Q: Can I check if a specific person is blocked from receiving data?**
Yes, you can use the `check_restriction_flags` tool to identify privacy barriers or 'No-Go' zones for a specific subject and recipient.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-communication-consent-map](https://vinkius.com/en/ai-agent-connect/care-communication-consent-map)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Communication & Consent Map** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-communication-consent-map` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Communication & Consent Map** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-communication-consent-map": {
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
