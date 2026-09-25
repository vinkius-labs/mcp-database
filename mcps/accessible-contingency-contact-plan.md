# Accessible Contingency Contact Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-contingency-contact-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Generates structured response protocols and contact summaries for access-dependent operations.

## Description
This MCP server provides specialized tools for managing contingency scenarios when critical access is lost. It allows users to `generate_contact_card` for rapid information retrieval, `draft_notification_messages` for stakeholder communication, `evaluate_fallback_plan` to identify pre-approved alternatives, and `get_update_procedure` to standardize post-incident documentation. It bridges the gap between service interruptions and organized escalation paths.


## Available Tools (4)
- **draft_notification_messages**: Generates tailored, scenario-specific messages for various stakeholders based on the interruption type
- **evaluate_fallback_plan**: Identifies the specific alternative actions and commitments that must be activated when an access-dependent activity is interrupted
- **generate_contact_card**: Creates a single-view summary of essential contact information for a specific person or entity within a contingency scenario
- **get_update_procedure**: Provides the standardized steps for documenting a contingency event and updating the contact plan after an interruption has been resolved


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Contingency Contact Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need the contact card for contact ID 'C-101' in scenario 'S-500'."

**🤖 AI Agent:**
> Contact Name: John Doe, Primary Channel: SMS, Details: +1-555-0199, Role: Tier 1 Responder, Priority: High.

---

**👤 You:**
> "Draft a notification for technical support regarding scenario 'S-500'."

**🤖 AI Agent:**
> Notification for Technical Support: An interruption has occurred in scenario S-500. Please review the current escalation status and prepare for activation.

---

**👤 You:**
> "What is the fallback plan for activity 'A-202' due to a hardware failure?"

**🤖 AI Agent:**
> Fallback Action: Switch to manual data entry via the secondary terminal. Commitment: Ensure all logs are synchronized within 2 hours. Trigger: Loss of primary hardware access.


## ❓ FAQ

**Q: How do I get contact details during an interruption?**
You can use the `generate_contact_card` tool to retrieve a structured summary of essential contact information for a specific person or entity.

**Q: Can I draft messages for my team?**
Yes, the `draft_notification_messages` tool generates tailored, professional messages for different recipient types like technical support or approvers.

**Q: What happens if a primary access method fails?**
You can use `evaluate_fallback_plan` to identify the specific alternative actions and commitments that must be activated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-contingency-contact-plan](https://vinkius.com/en/ai-agent-connect/accessible-contingency-contact-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Contingency Contact Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-contingency-contact-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Contingency Contact Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-contingency-contact-plan": {
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
