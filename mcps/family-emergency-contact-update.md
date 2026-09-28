# Family Emergency Contact Update MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-emergency-contact-update)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and synchronize emergency contact data across multiple institutions with consent-aware validation.

## Description
This MCP server provides a specialized management system for processing institutional emergency contact data. It ensures that all contact information is compliant with specific organizational requirements and respects complex consent hierarchies. Users can use `generate_update_packet` to create submission-ready data, `calculate_submission_sequence` to determine the optimal order of updates based on legal priority, `create_verification_checklist` to audit contact validity, and `generate_reminder_schedule` to maintain a proactive annual review calendar.


## Available Tools (4)
- **create_verification_checklist**: Generates a list of tasks to ensure all emergency contact information is legally and practically sound
- **generate_reminder_schedule**: Produces a yearly calendar of dates when contact information should be reviewed
- **calculate_submission_sequence**: Determines the optimal order for submitting updates across multiple institutions
- **generate_update_packet**: Creates a formatted data package ready for submission to a specific institution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Emergency Contact Update** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an update packet for Westside Hospital using these contacts and requirements."

**🤖 AI Agent:**
> The update packet for Westside Hospital has been generated. It includes the validated contact details for the primary Medical Proxy and meets all mandatory field requirements.

---

**👤 You:**
> "What is the best order to update my contacts for the school and the hospital?"

**🤖 AI Agent:**
> The optimal sequence is to update the hospital first to establish legal authority, followed by the school.

---

**👤 You:**
> "Create a checklist to verify my emergency contacts."

**🤖 AI Agent:**
> The verification checklist is ready. It includes tasks for field completeness, role-based permission validation, and consent hierarchy adherence.


## ❓ FAQ

**Q: How does the system handle conflicting contact permissions?**
The system applies a consent precedence logic where the highest-ranking role, such as a Medical Proxy, overrides permissions from lower-tier contacts.

**Q: Can I prepare data for multiple institutions at once?**
Yes, you can use `calculate_submission_sequence` to organize multiple update packets into a logical order for submission.

**Q: How are annual reminders managed?**
You can use `generate_reminder_schedule` to create a recurring calendar based on institutional deadlines and a preferred lead time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-emergency-contact-update](https://vinkius.com/en/ai-agent-connect/family-emergency-contact-update)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Emergency Contact Update** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-emergency-contact-update` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Emergency Contact Update** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-emergency-contact-update": {
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
