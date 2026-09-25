# Care Emergency Contact Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-emergency-contact-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-response](../categories/emergency-response.md)

Manage emergency contacts, notification sequences, and information-sharing boundaries.

## Description
This MCP server provides a structured framework for managing emergency contact protocols. It allows AI agents to generate printable contact cards using `get_contact_card`, calculate escalation paths via `generate_notification_sequence`, verify data access permissions with `check_information_boundaries`, and track mandatory quarterly audits through `get_review_schedule`. It ensures critical information reaches the right people in the correct order during emergencies.


## Available Tools (4)
- **get_review_schedule**: Provides the user with their next required contact plan audit to ensure data integrity
- **check_information_boundaries**: Determines what specific information is permitted to be shared with a given contact based on their role
- **generate_notification_sequence**: Calculates the step-by-step escalation path to be followed during an emergency
- **get_contact_card**: Generates a formatted, printable summary of a specific authorized contact for quick reference


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Emergency Contact Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a contact card for contact ID 'user-123'."

**🤖 AI Agent:**
> Name: Jane Doe, Role: Spouse, Method: Phone Call, Number: +1-555-0101, Location: New York, USA

---

**👤 You:**
> "What is the notification sequence for an 'Immediate' priority emergency?"

**🤖 AI Agent:**
> 1. John Doe (Phone Call), 2. Mary Smith (SMS), 3. Local Police (Voice).

---

**👤 You:**
> "Can a neighbor receive medical details during a 'Medical' incident?"

**🤖 AI Agent:**
> No, for a 'Medical' incident, a neighbor is restricted to notification only and cannot access sensitive medical data.


## ❓ FAQ

**Q: How can I see the contact details for a specific person?**
You can use the `get_contact_card` tool by providing the specific contact ID to generate a printable summary.

**Q: How does the notification order work?**
The system uses `generate_notification_sequence` to follow a strict call-tree hierarchy, ensuring contacts are reached in the correct priority order.

**Q: How often should I review my contact plan?**
The plan requires a quarterly review. You can check your next scheduled audit using `get_review_schedule`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-emergency-contact-plan](https://vinkius.com/en/ai-agent-connect/care-emergency-contact-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Emergency Contact Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-emergency-contact-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Emergency Contact Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-emergency-contact-plan": {
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
