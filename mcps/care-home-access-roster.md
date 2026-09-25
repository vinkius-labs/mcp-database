# Care Home Access Roster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-home-access-roster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Manage visitor authorization, entry methods, and safety protocols for care facilities.

## Description
This MCP server provides tools to manage secure visitor access in care facilities. It allows staff to retrieve the current access roster using `get_access_roster`, generate personalized entry guidance via `generate_arrival_instructions`, and manage security through `create_revocation_task` and `validate_visitor_workflow`. It ensures that all entries are authorized within specific visit windows and comply with building rules and privacy boundaries.


## Available Tools (4)
- **create_revocation_task**: Initiates the immediate removal of a visitor's access and triggers the necessary safety workflows
- **generate_arrival_instructions**: Creates a personalized set of instructions for a specific visitor to ensure a smooth and compliant entry
- **get_access_roster**: Provides a comprehensive list of all currently authorized visitors and their scheduled arrival/departure information
- **validate_visitor_workflow**: Executes a multi-step confirmation process to verify a visitor's identity and authorization at the point of entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Home Access Roster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current list of authorized visitors for facility ID 'CH-9921'."

**🤖 AI Agent:**
> The current access roster for facility CH-9921 includes 3 authorized visitors: John Doe (Keypad, 09:00-11:00), Jane Smith (Biometric, 13:00-15:00), and Robert Brown (Keypad, 14:00-16:00).

---

**👤 You:**
> "Generate entry instructions for visitor 'V-442' at facility 'CH-9921'."

**🤖 AI Agent:**
> Visitor Jane Smith: Please use the biometric scanner at the North Entrance. Ensure you follow all quiet hour protocols and remain within the designated resident common areas.

---

**👤 You:**
> "Revoke access for visitor 'V-101' at facility 'CH-9921' due to policy violation."

**🤖 AI Agent:**
> Revocation task for visitor V-101 has been successfully initiated. Entry methods are invalidated and emergency contacts have been notified.


## ❓ FAQ

**Q: How can I see who is currently allowed in the facility?**
You can use the `get_access_roster` tool to retrieve a real-time list of all authorized visitors and their scheduled windows.

**Q: What happens if a visitor's access needs to be cancelled immediately?**
Use the `create_revocation_task` tool to immediately invalidate entry methods and notify emergency contacts.

**Q: Can this tool help with visitor identity verification?**
Yes, the `validate_visitor_workflow` tool executes a multi-step confirmation process to verify identity and authorization at the point of entry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-home-access-roster](https://vinkius.com/en/ai-agent-connect/care-home-access-roster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Home Access Roster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-home-access-roster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Home Access Roster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-home-access-roster": {
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
