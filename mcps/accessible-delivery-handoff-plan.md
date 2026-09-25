# Accessible Delivery Handoff Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-delivery-handoff-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synthesize delivery provider constraints with user accessibility needs to generate actionable handoff instructions and workflows.

## Description
This MCP server bridges the gap between delivery logistics and personal accessibility requirements. It allows AI agents to reconcile provider constraints (like FedEx or UPS capabilities) with user-defined needs such as drop locations, weight limits, and authorization levels. Use `generate_delivery_instructions` to create driver-ready text, `create_confirmation_workflow` to define driver steps, `generate_escalation_messages` for failed attempts, and `build_provider_setup_checklist` to manage multi-provider configurations.


## Available Tools (4)
- **generate_delivery_instructions**: Creates specific text instructions for a driver to ensure a successful, accessible handoff
- **build_provider_setup_checklist**: Generates a checklist for the user to ensure their delivery profiles are correctly configured
- **create_confirmation_workflow**: Defines the step-by-step operational sequence for a driver to follow to confirm a successful handoff
- **generate_escalation_messages**: Produces messages to be sent to the user or a secondary contact if a delivery attempt fails


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Delivery Handoff Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate delivery instructions for a 5kg package being delivered by FedEx to my front porch."

**🤖 AI Agent:**
> Please leave the 5kg package at the front porch. Ensure it is placed securely away from the walkway.

---

**👤 You:**
> "Create a confirmation workflow for a secure location requiring a signature via SMS."

**🤖 AI Agent:**
> 1. Verify access to the secure location. 2. Contact the resident via SMS. 3. Obtain the required signature. 4. Confirm delivery.

---

**👤 You:**
> "What should I do if the delivery failed because the weight limit was exceeded?"

**🤖 AI Agent:**
> The delivery could not be completed because the item weight exceeds your specified handling limit. Please contact the provider to arrange a different handoff method.


## ❓ FAQ

**Q: How do I generate instructions for a specific driver?**
You can use the `generate_delivery_instructions` tool by providing the provider name, the chosen drop location, and the item weight.

**Q: Can this tool handle failed delivery attempts?**
Yes, the `generate_escalation_messages` tool produces ready-to-send messages for users or contacts when a handoff fails.

**Q: How do I ensure my delivery profiles are consistent?**
Use the `build_provider_setup_checklist` tool to generate a configuration task list for all your selected delivery providers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-delivery-handoff-plan](https://vinkius.com/en/ai-agent-connect/accessible-delivery-handoff-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Delivery Handoff Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-delivery-handoff-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Delivery Handoff Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-delivery-handoff-plan": {
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
