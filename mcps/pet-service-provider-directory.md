# Pet Service Provider Directory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-service-provider-directory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [pet-care](../categories/pet-care.md)

Manage approved pet service providers with privacy safeguards and maintenance workflows.

## Description
This MCP server provides a managed system for organizing approved pet service providers. It allows users to access a structured directory via `get_provider_directory`, retrieve optimal contact methods based on urgency using `get_provider_contact_details`, and verify data privacy through `get_information_sharing_checklist`. It also includes operational tools like `get_maintenance_and_review_plan` to manage directory upkeep and scheduled audits.


## Available Tools (4)
- **get_information_sharing_checklist**: Generates a list of data points that are cleared to be shared with a specific provider
- **get_maintenance_and_review_plan**: Provides the operational roadmap for directory upkeep and scheduled audits
- **get_provider_contact_details**: Retrieves the optimal contact information for a specific provider based on the required service urgency
- **get_provider_directory**: Returns a structured list of all approved providers organized by the user's custom categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Service Provider Directory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all providers in the Emergency category."

**🤖 AI Agent:**
> Here are the providers in the Emergency category: Dr. Bark (Vet), QuickPaws (Walker), and PetRescue (Emergency Vet).

---

**👤 You:**
> "I need to contact Dr. Bark immediately for an emergency."

**🤖 AI Agent:**
> The primary contact for Dr. Bark is 555-0123 (Phone).

---

**👤 You:**
> "What information can I share with QuickPaws?"

**🤖 AI Agent:**
> You can share contact details with QuickPaws, but medical history and home access are currently restricted.


## ❓ FAQ

**Q: How can I see all available pet service providers?**
You can use the `get_provider_directory` tool to see a structured list of all approved providers, which can be filtered by your custom categories.

**Q: How does the system handle emergency contact information?**
When you indicate a service is urgent, `get_provider_contact_details` prioritizes contact methods with the lowest response latency, such as phone calls.

**Q: How is my pet's private information protected?**
Privacy is enforced through the `get_information_sharing_checklist` tool, which only shows data points that the specific provider is explicitly authorized to receive.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-service-provider-directory](https://vinkius.com/en/ai-agent-connect/pet-service-provider-directory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Service Provider Directory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-service-provider-directory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Service Provider Directory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-service-provider-directory": {
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
