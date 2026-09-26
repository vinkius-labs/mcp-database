# Emergency Accessibility Support Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-accessibility-support-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Transforms accessibility needs and local resources into actionable emergency response plans and contact cards.

## Description
This MCP server provides a specialized coordination engine for emergency preparedness. It converts functional access needs into structured coordination plans, high-readability contact cards for responders, and equipment ownership registries. Users can use `generate_coordination_plan` to align needs with local resources, `create_contact_card` to prepare vital information for first responders, `list_supply_ownership` to manage accessibility equipment, and `generate_practice_schedule` to establish regular safety drills.


## Available Tools (4)
- **create_contact_card**: Generates a simplified, high-priority information card for immediate use by responders
- **generate_coordination_plan**: Creates a personalized emergency response strategy by reconciling user needs with local official resources
- **generate_practice_schedule**: Produces a training timeline to ensure the user and contacts can execute the support plan
- **list_supply_ownership**: Clarifies who is responsible for which pieces of accessibility equipment during an emergency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Accessibility Support Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a coordination plan for someone needing mobility assistance and visual aids, using local EMS and transit services."

**🤖 AI Agent:**
> The coordination plan has been generated. It aligns your mobility and visual needs with the available local EMS and transit protocols, ensuring transport is compatible with your requirements.

---

**👤 You:**
> "Create a contact card for my emergency contacts and my functional needs."

**🤖 AI Agent:**
> Your contact card is ready. It contains your vital functional needs and the contact details for your authorized individuals, while strictly adhering to your privacy instructions.

---

**👤 You:**
> "List who is responsible for my wheelchair and hearing aid."

**🤖 AI Agent:**
> The ownership registry shows that the wheelchair is maintained by the user and the hearing aid is maintained by the primary caregiver.


## ❓ FAQ

**Q: How does the coordination plan handle conflicting information?**
The system follows a strict precedence hierarchy: user consent is prioritized first, followed by official local guidance, and finally instructions from trusted support contacts.

**Q: Can I use this to get a medical diagnosis?**
No. This tool is strictly non-diagnostic. It only processes functional access needs to create safety plans and does not identify or suggest medical conditions.

**Q: What is included in the contact card?**
The contact card provides a high-priority summary for responders, including vital functional needs, authorized contact lists, and privacy instructions based on your consent preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-accessibility-support-plan](https://vinkius.com/en/ai-agent-connect/emergency-accessibility-support-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Accessibility Support Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-accessibility-support-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Accessibility Support Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-accessibility-support-plan": {
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
