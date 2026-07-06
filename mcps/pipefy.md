# Pipefy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipefy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Manage workflows via Pipefy — list pipes, create cards, move phases, update fields, and track processes directly from any AI agent.

## Description
Connect your **Pipefy** account to any AI agent and take full control of your process management workflows through natural conversation.

### What you can do

- **Pipe Discovery** — List all pipes (processes) in your organization and inspect their structure, phases, and fields
- **Card Management** — Create, read, update, and delete cards (items/records) flowing through your pipes
- **Field Updates** — Update specific field values on existing cards as information changes or processes evolve
- **Phase Transitions** — Move cards between phases to advance workflow steps (e.g., New → In Progress → Done)
- **Card Search** — Search for cards by field value to find specific items by email, name, ID, or custom data
- **Card Cloning** — Duplicate existing cards to quickly create similar items with pre-filled field values
- **Organization Info** — View organization details, members, and available pipes
- **User Profile** — Check your authenticated user profile and organization memberships

### How it works

1. Subscribe to this server
2. Enter your Pipefy API token (from Profile > API Access or Service Accounts)
3. Start managing your workflows from Claude, Cursor, or any MCP-compatible client

No more navigating the Pipefy dashboard for every workflow action. Your AI acts as a dedicated process manager.

### Who is this for?

- **Operations Teams** — instantly create cards, move them through phases, and update fields without opening the Pipefy dashboard
- **Project Managers** — monitor card progress across multiple pipes and identify bottlenecks in workflows
- **Support Staff** — search for cards by customer email or ID to quickly find and update related requests
- **Process Owners** — clone cards for recurring processes and manage field values as requests evolve


## Available Tools (14)
- **clone_card**: You must provide the card_id of the card to clone.
The new card is created in the same pipe as the original, starting at the first phase.
This is useful for creating similar requests, repeating processes, or using an existing card 
as a template for new items. The cloned card gets a new unique ID but retains all field data.

Clone an existing card to create a duplicate
- **get_user_profile**: Use this to verify API token access and discover organization IDs needed for other queries.
This is also useful for understanding which organizations and pipes the user has access to.

Get the authenticated user profile
- **create_card**: You must provide the pipe_id and 
a JSON object containing field values matching the pipe's required fields.
Fields are key-value pairs where keys are field IDs and values are the data to store.
Optionally specify a phase_id to start the card in a specific phase (defaults to first phase).
Example fields: { "name": "John Doe", "email": "john@example.com", "priority": "High" }

Create a new card in a Pipefy pipe
- **delete_card**: You must provide the card_id.
This action cannot be undone. Use this to remove test cards, duplicates, or items that were 
created in error. Be careful as this will also remove all associated data including comments,
attachments, and field values for that card.

Delete a card from a pipe
- **get_card**: Use the card_id obtained from list_cards to inspect full card information.
This is useful for reviewing card details before updating fields or moving to another phase.

Get detailed information about a specific card
- **get_organization**: Use the organization_id to inspect your organization's structure, understand team membership,
and discover available pipes for card management.

Get details of a Pipefy organization
- **get_phase**: Phases represent steps in a pipe's workflow.
Use the phase_id obtained from get_pipe or list_phases to inspect phase configuration.
This helps understand what fields are required at each step of the workflow.

Get details of a specific phase
- **get_pipe**: Each pipe represents a workflow or process with multiple phases (steps) and custom fields.
Use the pipe_id to get the structure of a pipe before creating cards or managing cards within it.
The response includes all phases with their IDs, names, and the custom fields defined for the pipe.

Get details of a specific Pipefy pipe (process)
- **list_cards**: Cards represent individual items 
flowing through the pipe's workflow phases (e.g., requests, tasks, tickets, leads).
You must provide the pipe_id. Optionally filter by phase_id to see cards in a specific phase.
Each card includes title, current phase, completion status, due date, and assignees.
Use this to monitor workflow progress and identify cards that need attention.

List all cards in a pipe with optional phase filter
- **list_phases**: Each phase represents a stage that cards flow through in the process.
Use this to understand the workflow structure and identify phase IDs for filtering cards
or moving cards between phases. The response includes phase names and card counts.

List all phases in a pipe
- **list_pipes**: Each pipe represents a structured workflow with phases, fields, and cards.
You must provide the organization_id which can be found in your Pipefy URL or obtained from get_user_profile.
Use this to discover all available pipes before managing cards within them.

List all pipes in an organization
- **move_card_to_phase**: You must provide the card_id and the target phase_id.
This is the primary way to advance workflow items through the pipe's process steps.
Common use cases: moving a request from "New" to "In Review", advancing a lead to "Qualified",
or progressing a task to "Completed". The card retains all its field values after moving.

Move a card to a different phase in the pipe
- **search_cards_by_field**: This is useful for finding cards by email, name, ID, or any custom field content.
You must provide the pipe_id, field_id (the field to search in), and search_value (text to find).
Results include card title, current phase, status, and all field values for matching cards.
The search uses a "contains" operator for flexible matching.

Search cards in a pipe by a specific field value
- **update_card_field**: You must provide the card_id, 
the field_id of the field to update, and the new value as a string.
This is useful for updating card information as requests progress or details change.
Common updates: changing priority, updating contact info, modifying descriptions, or setting dates.

Update a specific field value on a card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipefy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pipes in my organization and show me the cards in the 'IT Support' pipe."

**🤖 AI Agent:**
> I've retrieved your organization's pipes. You have 5 active pipes: 'IT Support', 'HR Onboarding', 'Purchase Requests', 'Bug Tracking', and 'Content Approval'. In the 'IT Support' pipe, I found 12 cards: 4 in 'New Requests', 5 in 'In Progress', and 3 in 'Waiting for User'. The oldest card has been waiting 5 days. Would you like the full details of any specific card?

---

**👤 You:**
> "Create a new purchase request card in the Purchase Requests pipe with these details: Requester: Maria Silva, Item: MacBook Pro 16", Quantity: 2, Justification: Design team replacement."

**🤖 AI Agent:**
> I've successfully created the purchase request card:
- **Card ID**: 12345678
- **Title**: Purchase Request - Maria Silva
- **Current Phase**: New Requests
- **Fields**: Requester: Maria Silva, Item: MacBook Pro 16", Quantity: 2, Justification: Design team replacement

The card is now in the 'New Requests' phase and ready for review. Would you like me to move it to 'Manager Approval' phase?

---

**👤 You:**
> "Search for all cards in the IT Support pipe where the email field contains 'john@company.com' and show me their current status."

**🤖 AI Agent:**
> I found 3 cards in the IT Support pipe for john@company.com:

1. **Card #12345** — 'Monitor not displaying' — Phase: In Progress — Created: 2024-04-01
2. **Card #12389** — 'Keyboard replacement request' — Phase: Waiting for Parts — Created: 2024-04-03
3. **Card #12401** — 'VPN access issue' — Phase: Resolved — Created: 2024-04-05

Two cards are still active (In Progress and Waiting for Parts), and one is resolved. Would you like the full details of any specific card?


## ❓ FAQ

**Q: How do I get a Pipefy API token and where do I find it?**
Log in to Pipefy, click on your **Profile icon** (top-right), go to **Profile > API Access**, and generate a new token. Alternatively, use **Service Accounts** for team-based access. Copy the token immediately — it starts with `eyJhbG...`. Paste it into the API token field below. This token authenticates all GraphQL API requests to `https://api.pipefy.com/graphql`.

**Q: How do I move a card from one phase to another in a pipe?**
Use the `move_card_to_phase` tool with the card_id (from list_cards or get_card) and the target phase_id (from get_pipe or list_phases). This advances the card through your workflow. For example, moving a card from 'New Requests' to 'In Review' phase. The card retains all its field values after moving. This is the primary way to progress items through your process.

**Q: Can I search for cards by a specific field value like email or customer name?**
Yes! Use the `search_cards_by_field` tool with the pipe_id, field_id (the specific field to search in), and search_value (the text to find). This searches all cards in the pipe where that field contains your search text. It's perfect for finding cards by customer email, name, order number, or any custom field. Results include full card details with all field values.

**Q: How do I create a new card with custom field values?**
Use the `create_card` tool with the pipe_id and a JSON object containing field values. The fields parameter should be a JSON object where keys are field IDs (from get_pipe) and values are the data to store. Example: `{ "name": "John Doe", "email": "john@example.com", "priority": "High" }`. You can also optionally specify a phase_id to start the card in a specific phase instead of the default first phase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipefy](https://vinkius.com/mcp/pipefy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipefy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipefy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipefy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipefy": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
