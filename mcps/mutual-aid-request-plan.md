# Mutual Aid Request Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mutual-aid-request-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [coordination](../categories/coordination.md)

A coordination engine that transforms individual support needs into structured, privacy-respecting community action plans.

## Description
This MCP server provides a coordination engine to transform individual support needs into structured, privacy-respecting community action plans. It manages the lifecycle of mutual aid requests using tools like `plan_request_structure` to organize needs, `generate_response_workflow` to define responder steps, `assign_helper_to_task` to establish task ownership, and `finalize_request_closure` to complete the process. The system enforces strict privacy boundaries and minimum disclosure rules, ensuring sensitive information is only shared with assigned helpers.


## Available Tools (4)
- **finalize_request_closure**: Marks a request as completed and generates the final communication for the coordination channel
- **generate_response_workflow**: Defines the step-by-step process for how a responder moves from seeing a request to completing it
- **plan_request_structure**: Converts raw user input into a structured, actionable mutual aid request
- **assign_helper_to_task**: Formally assigns a specific helper to a specific task within the request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mutual Aid Request Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need help getting groceries this Thursday in the downtown area. I'm okay with people leaving them on my porch. My contact is Jane at 555-0123."

**🤖 AI Agent:**
> I have created a structured mutual aid request for grocery support in the downtown area for this Thursday, including your privacy boundary to leave items on the porch.

---

**👤 You:**
> "Show me the steps I need to follow to help with the grocery request."

**🤖 AI Agent:**
> The workflow includes: 1. Discovery, 2. Opt-in Commitment, 3. Information Disclosure, 4. Task Execution, and 5. Closure.

---

**👤 You:**
> "Assign Mark to the grocery delivery task for request ID 123."

**🤖 AI Agent:**
> Mark has been successfully assigned as the Owner of the grocery delivery task for request 123.


## ❓ FAQ

**Q: How does this tool protect my privacy?**
The system uses Minimum Disclosure rules. Sensitive contact information is only revealed to a helper once they have been formally assigned to a task via `assign_helper_to_task`.

**Q: Can I choose not to help if I see a request?**
Yes. The system follows Opt-in Participation principles. Responders can view requests but are under no obligation to commit unless they explicitly choose to.

**Q: What happens once a helper accepts a task?**
Once a helper is assigned using `assign_helper_to_task`, they become the 'Owner' of that task and are responsible for its execution and status updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mutual-aid-request-plan](https://vinkius.com/en/ai-agent-connect/mutual-aid-request-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mutual Aid Request Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mutual-aid-request-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mutual Aid Request Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mutual-aid-request-plan": {
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
