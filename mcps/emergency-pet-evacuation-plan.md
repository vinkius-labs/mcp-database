# Emergency Pet Evacuation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-pet-evacuation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Coordinate pet evacuations by managing readiness, packing, and logistics.

## Description
This MCP server provides the essential tools for managing pet evacuations during emergencies. It allows AI agents to use `check_evacuation_readiness` to verify pet documentation, `generate_packing_list` to prepare supplies, `calculate_logistics_plan` to organize transport and carriers, and `get_caretaker_contacts` to identify authorized personnel at destinations.


## Available Tools (4)
- **calculate_logistics_plan**: Determines the optimal order of operations and carrier requirements to move all pets
- **check_evacuation_readiness**: Determines if a specific pet is cleared for evacuation based on documentation and destination rules
- **generate_packing_list**: Creates a checklist of supplies needed for each pet based on their dietary and medical needs
- **get_caretaker_contacts**: Retrieves the contact information for individuals authorized to handle the pets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Pet Evacuation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is pet_123 ready to be evacuated to destination_abc?"

**🤖 AI Agent:**
> Pet_123 is ready for evacuation to destination_abc.

---

**👤 You:**
> "What supplies do I need to pack for pet_456 and pet_789?"

**🤖 AI Agent:**
> For pet_456, you need 5kg of dry food and a medical kit. For pet_789, you need 3kg of dry food and specialized water supplies.

---

**👤 You:**
> "Who can I contact at destination_xyz to receive the pets?"

**🤖 AI Agent:**
> The authorized contacts at destination_xyz are Jane Doe (Primary Caretaker) at 555-0123 and John Smith (Transport Coordinator) at 555-0456.


## ❓ FAQ

**Q: How do I know if a pet is ready to be moved?**
You can use the `check_evacuation_readiness` tool to verify if a pet's veterinary records are valid and if the destination can accept their species.

**Q: Can I plan the transport for multiple pets at once?**
Yes, the `calculate_logistics_plan` tool helps determine the sequence of steps and carrier assignments for a group of pets.

**Q: How are packing lists generated?**
The `generate_packing_list` tool creates a checklist of food, water, and medical supplies based on the specific needs of the pets provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-pet-evacuation-plan](https://vinkius.com/en/ai-agent-connect/emergency-pet-evacuation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Pet Evacuation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-pet-evacuation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Pet Evacuation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-pet-evacuation-plan": {
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
