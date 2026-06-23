# Elvanto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elvanto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Elvanto church database — search people, update profiles, and coordinate people flows directly from your AI agent.

## Description
Connect your **Elvanto** account to any AI agent to manage your church database and people flows through natural conversation.

### What you can do

- **People Management** — List, search, retrieve, create, edit, and remove people profiles in your database.
- **Custom Fields & Categories** — Access custom fields and people categories to keep your directory organized.
- **People Flows** — Track progress by listing flows, steps, and members within specific steps, or add people to flows.
- **User Insights** — Retrieve details about the currently logged-in API user.

### How it works

1. Subscribe to this server
2. Enter your Elvanto API Key
3. Start managing your directory from Claude, Cursor, or any MCP-compatible client


## Available Tools (46)
- **add_group_person**: Add a person to a group, or change their position
- **add_person_to_flow_step**: Adds a person to a specified People Flow Step
- **create_calendar_event**: Create a new calendar event
- **create_financial_category**: Creates a new category in the Chart of Accounts
- **create_group**: Create a new group
- **create_person**: Create a new person
- **create_song_arrangement**: Create an arrangement tied to a specified song
- **create_song_key**: Create a key attached to a specified arrangement
- **create_song**: Create a new song
- **create_transaction**: Create a new transaction
- **edit_calendar_event**: Edit an existing calendar event
- **edit_group**: Edit an existing group
- **edit_person**: Edit an existing person
- **edit_song_arrangement**: Edit a specific arrangement details
- **edit_song_key**: Edit an existing key
- **edit_song**: Edit specific details about a chosen song
- **edit_transaction**: Edit an existing transaction
- **get_current_user**: Retrieve information of the logged-in user
- **get_group**: Find a group based on its ID
- **get_person**: Find a person based on their ID
- **get_service**: Find a service based on its ID
- **get_song_arrangement**: Find an arrangement based on its ID
- **get_song_key**: Find a key based on its ID
- **get_song**: Find a song based on its ID
- **get_transaction**: Find a transaction based on its ID
- **list_calendar_events**: Get a list of all events between two dates
- **list_calendars**: Get a list of all Calendars that events can be assigned to
- **list_custom_fields**: Get a list of all Custom Fields
- **list_financial_categories**: Get a list of all Chart of Accounts categories
- **list_groups**: Get a list of all groups
- **list_people_categories**: Get a list of all People Categories
- **list_people_flow_step_people**: Lists members inside a specific People Flow step
- **list_people_flow_steps**: Lists all People Flow Steps within a given People Flow
- **list_people_flows**: Lists all People Flows in the account
- **list_people**: Get a list of all people
- **list_services**: Get a list of services
- **list_song_arrangements**: Get a list of arrangements within a song
- **list_song_keys**: Get a list of keys within an arrangement
- **list_songs**: Get a list of songs
- **list_transactions**: Get a list of all transactions between two dates
- **remove_calendar_event**: Delete a calendar event
- **remove_group_person**: Remove a person from a group
- **remove_group**: Delete a group
- **remove_person**: Delete a person
- **remove_transaction**: Delete a transaction
- **search_people**: Find one or more people matching a specific search query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elvanto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all male volunteers in our database."

**🤖 AI Agent:**
> I will use the `search_people` tool with the search criteria `{"gender": "Male", "volunteer": "yes"}` to find matching profiles.

---

**👤 You:**
> "List all active People Flows in our Elvanto account."

**🤖 AI Agent:**
> I will call the `list_people_flows` tool to retrieve all configured people flows and their details.

---

**👤 You:**
> "Get the profile details for person ID 12345."

**🤖 AI Agent:**
> I will use the `get_person` tool with ID `12345` to fetch their complete profile information.


## ❓ FAQ

**Q: How can I search for a specific person in my Elvanto database?**
You can use the `search_people` tool. Provide search criteria as key-value pairs (for example, `{"volunteer": "yes"}`) to find matching profiles instantly.

**Q: Can I add a person to a specific step in a People Flow?**
Yes! Use the `add_person_to_flow_step` tool by passing the target `step_id` and the `person_id` to assign them to that flow step.

**Q: How do I view all custom fields configured in my account?**
Simply ask the agent to run the `list_custom_fields` tool. It will retrieve all custom fields defined in your Elvanto account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elvanto](https://vinkius.com/mcp/elvanto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elvanto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elvanto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elvanto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elvanto": {
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
