# Trello MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trello)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate project management via Trello — list boards, manage lists, and inspect or create cards directly from any AI agent.

## Description
Connect your **Trello** organizational account to any AI agent and take full control of your agile project management workflows through natural conversation.

### What you can do

- **Boards & Lists** — Fetch all your active boards and inspect the lists (columns) organizing your workflow directly from the Trello cloud
- **Card Management** — Query all cards from any target list or search across the board using unique IDs
- **Deep Card Inspection** — Fetch complete metadata, descriptions, assignee fields, due dates, and exact status metrics for specific individual cards
- **Workflow Automation** — Create new cards on the fly, update existing ones, or easily move them between lists inside your agent
- **User Profiling** — Retrieve the underlying credentials and profile information for your Trello workspace members

### How it works

1. Subscribe to this server
2. Enter your Trello API Key and Token
3. Start managing your kanban boards from Claude, Cursor, or any MCP-compatible client

No more wrestling with hundreds of open browser tabs to find out who is assigned to a specific task block. Your AI acts as a dedicated Scrum master or project manager.

### Who is this for?

- **Product Managers** — instantly retrieve project statuses, list stale cards, and inspect sprint boards without opening the Trello app
- **Engineering Teams** — check task descriptions and priorities straight from the code editor to avoid breaking flow
- **Operations & Agency Leads** — automate client workspace querying and smoothly transition cards across completion stages


## Available Tools (16)
- **add_checklist**: You can then add check items to it via the Trello UI.

Add a new checklist to a Trello card
- **add_comment**: Comments appear in the card activity feed and notify watchers.

Add a comment to a Trello card
- **add_label_to_card**: Use list_labels to get available label IDs for the board.

Add a label to a Trello card
- **create_card**: Create a new Trello card
- **delete_card**: Prefer updating closed to true for archiving instead.

Permanently delete a Trello card
- **get_board**: Get details for a specific Trello board
- **get_card**: Get details for a specific Trello card
- **get_me**: Get current Trello user details
- **list_board_cards**: Useful for getting a complete board overview.

List all cards across all lists in a Trello board
- **list_boards**: List Trello boards for the user
- **list_cards**: List cards in a specific Trello list
- **list_labels**: Use label IDs with add_label_to_card.

List all labels for a Trello board
- **list_lists**: List lists (columns) in a Trello board
- **list_members**: List members of a Trello board
- **search_cards**: Returns matching cards with board and list context.

Search for Trello cards by keyword
- **update_card**: Update an existing Trello card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trello** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the boards under my Trello account right now."

**🤖 AI Agent:**
> I've retrieved your boards. You currently operate 'Development Sprints' (ID: 64fa8211), 'Content Marketing' (ID: 64ea9bc), and 'IT Tickets'. Which one should we dive into?

---

**👤 You:**
> "Can you check the cards currently inside the 'To Do' list ID 618ab221?"

**🤖 AI Agent:**
> Running the extraction... I found 4 cards currently in 'To Do'. These include 'Update Auth Module' (ID: 63ab), 'Setup DB Indexes' (ID: 6511), and two others. Would you like to read the details for the Auth task?

---

**👤 You:**
> "Create a new board card called 'Verify Webhooks' with the description 'Check timeout limits under high load' on list 618ab221."

**🤖 AI Agent:**
> Task accomplished. 'Verify Webhooks' has been successfully created with an attached ID of 660f9a2bccd. Feel free to ask if you need to fetch its timeline or update the card further.


## ❓ FAQ

**Q: Can my AI automatically gather details of a specific card by its ID?**
Yes! Use the `get_card` tool with exactly the Card ID. Your agent will respond with complete metadata, assignee fields, standard labels, and precise notes within seconds.

**Q: How do I move a card from 'To Do' to 'Done' seamlessly?**
Simply ask the agent to run the `update_card` tool. Provide the Card ID and set the destination List ID (which you can find using `list_lists` first). The card will be moved across columns instantly.

**Q: Does the integration allow completely destructive operations like deleting my entire board?**
No. The agent is limited to safe mutations related to Cards—creating, updating, and removing cards. It does not contain tools to delete large configurations like Boards or Columns, protecting your company’s structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trello](https://vinkius.com/mcp/trello)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trello** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trello` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trello** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trello": {
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
