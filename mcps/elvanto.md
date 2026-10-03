# Elvanto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/elvanto)
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
- **add_group_person**: Specify the unique Group ID and Person ID.

Add a person to a group, or change their position
- **add_person_to_flow_step**: Adds a person to a specified People Flow Step
- **create_calendar_event**: Provide the name and required dates.

Create a new calendar event
- **create_financial_category**: Provide the category name.

Creates a new category in the Chart of Accounts
- **create_group**: You must provide a name for the new group.

Create a new group
- **create_person**: Provide at least a first name and last name.

Create a new person
- **create_song**: Provide a title and optionally a CCLI number.

Create a new song
- **create_song_arrangement**: Provide the song ID and arrangement name.

Create an arrangement tied to a specified song
- **create_song_key**: Provide the arrangement ID and key name.

Create a key attached to a specified arrangement
- **create_transaction**: Specify the person, date, and amounts.

Create a new transaction
- **edit_calendar_event**: Supply the event ID and the fields to be updated.

Edit an existing calendar event
- **edit_group**: Specify the unique group ID to modify the group.

Edit an existing group
- **edit_person**: Must specify the person’s ID.

Edit an existing person
- **edit_song**: Must provide both the song ID and the new title.

Edit specific details about a chosen song
- **edit_song_arrangement**: Must provide the arrangement ID.

Edit a specific arrangement details
- **edit_song_key**: Must provide the key ID.

Edit an existing key
- **edit_transaction**: Provide the transaction ID and the amounts to modify.

Edit an existing transaction
- **get_current_user**: This tool does not require any parameters.

Retrieve information of the logged-in user
- **get_group**: Provide the unique group ID.

Find a group based on its ID
- **get_person**: Pass the person’s unique ID.

Find a person based on their ID
- **get_service**: Provide the ID and optionally specify fields to retrieve.

Find a service based on its ID
- **get_song**: Optionally request attached files.

Find a song based on its ID
- **get_song_arrangement**: Provide the arrangement ID to proceed.

Find an arrangement based on its ID
- **get_song_key**: Provide the key ID to proceed.

Find a key based on its ID
- **get_transaction**: Provide the transaction ID.

Find a transaction based on its ID
- **list_calendar_events**: Provide start and end dates.

Get a list of all events between two dates
- **list_calendars**: Get a list of all Calendars that events can be assigned to
- **list_custom_fields**: This tool does not require any parameters.

Get a list of all Custom Fields
- **list_financial_categories**: Specify the page number if needed.

Get a list of all Chart of Accounts categories
- **list_groups**: Use category_id to filter results.

Get a list of all groups
- **list_people**: Use category_id to filter results if needed.

Get a list of all people
- **list_people_categories**: This tool does not require any parameters.

Get a list of all People Categories
- **list_people_flows**: This tool does not require any parameters.

Lists all People Flows in the account
- **list_people_flow_step_people**: Provide the step_id to scope the search.

Lists members inside a specific People Flow step
- **list_people_flow_steps**: Provide the flow_id as a parameter.

Lists all People Flow Steps within a given People Flow
- **list_services**: Specify date ranges or status filters if needed.

Get a list of services
- **list_song_arrangements**: Use this when you know the song ID.

Get a list of arrangements within a song
- **list_song_keys**: Use this when you know the arrangement ID.

Get a list of keys within an arrangement
- **list_songs**: Specify the desired page, page size, and search criteria.

Get a list of songs
- **list_transactions**: Provide both start and end dates.

Get a list of all transactions between two dates
- **remove_calendar_event**: Use the unique event ID for deletion.

Delete a calendar event
- **remove_group**: Provide the unique group ID to confirm deletion.

Delete a group
- **remove_group_person**: Provide both the Group ID and the Person ID.

Remove a person from a group
- **remove_person**: the deletion.

Delete a person
- **remove_transaction**: Use the unique transaction ID.

Delete a transaction
- **search_people**: Always provide a search query in the ’search’ parameter.

Find one or more people matching a specific search query


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

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/elvanto](https://vinkius.com/en/ai-agent-connect/elvanto)
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
