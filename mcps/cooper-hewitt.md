# Cooper Hewitt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cooper-hewitt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the Cooper Hewitt Smithsonian Design Museum collection — search objects, explore exhibitions, and retrieve detailed metadata about design history.

## Description
Connect to the **Cooper Hewitt Smithsonian Design Museum** API and explore one of the world's most comprehensive design collections directly through your AI agent.

### What you can do

- **Search the Collection** — Find objects, people, and media using keywords, colors, or specific time periods via `search_collection` and `search_objects`.
- **Object Details** — Retrieve rich metadata, including descriptions, participants, exhibition history, and color palettes using `get_object_info` and `get_object_colors`.
- **Visual Exploration** — Access high-quality images and visual assets for design research with `get_object_images`.
- **On Display** — See what is currently featured in the museum's physical galleries using `get_objects_on_display`.
- **Random Discovery** — Get inspired by pulling random objects from the vast archive with `get_random_object`.

### How it works

1. Subscribe to this server
2. Enter your Cooper Hewitt API Access Token
3. Start exploring design history from Claude, Cursor, or any MCP-compatible client

No more manual searching through web archives. Your AI acts as a specialized design historian and researcher.

### Who is this for?

- **Designers & Creatives** — find inspiration and historical context for projects directly in your workflow
- **Researchers & Students** — extract precise metadata and exhibition histories for academic or professional study
- **Developers** — integrate rich cultural heritage data into applications without complex API wrappers


## Available Tools (22)
- **get_exhibition_info**: Return detailed information for an exhibition
- **get_exhibition_objects**: Return objects displayed in an exhibition
- **get_object_colors**: Return the color palette for an object
- **get_object_exhibitions**: Return exhibitions featuring an object
- **get_object_images**: Return images for an object
- **get_object_info**: Return detailed information for a specific object
- **get_object_participants**: Return people involved with an object
- **get_objects_on_display**: Return a list of objects currently on display
- **get_person_images**: Return images of a person
- **get_person_info**: Return detailed information for a person
- **get_person_objects**: Return objects associated with a person
- **get_random_object**: Return a random object from the collection
- **list_exhibitions**: Return a list of exhibitions
- **list_rooms**: List all rooms across locations
- **list_sites**: List all location sites
- **search_collection**: Search for things in the collection
- **search_objects_faceted**: Search for objects and return faceted results
- **search_objects**: Search specifically for objects
- **spec_formats**: Return the list of valid API response formats
- **spec_methods**: Return the list of available API response methods
- **test_echo**: A testing method which echoes all parameters back in the response
- **test_error**: Return a test error from the API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cooper Hewitt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for objects in the collection related to 'Bauhaus' that have images."

**🤖 AI Agent:**
> I've searched the collection for 'Bauhaus' items with images. I found several objects, including a 1923 wallpaper sample (ID: 18491569) and a tea infuser. Would you like to see the detailed metadata or images for any of these?

---

**👤 You:**
> "Give me the color palette for object ID 18639529."

**🤖 AI Agent:**
> Fetching the color profile for object 18639529... The palette includes 'Vivid Tangerine' (#FF9F80), 'Dark Charcoal' (#333333), and 'Light Gray' (#D3D3D3).

---

**👤 You:**
> "Show me a random object from the museum to inspire my next design project."

**🤖 AI Agent:**
> Here is a random selection: 'Bird and Anemone' textile (1882), designed by William Morris. It's a block-printed cotton fabric featuring intricate floral and avian patterns. Would you like to see its exhibition history?


## ❓ FAQ

**Q: Can I search for objects by a specific color?**
Yes! Use the `search_collection` tool and provide a hex color or CSS name in the `color` parameter to find items matching that aesthetic.

**Q: How do I find out who designed a specific object?**
Use the `get_object_participants` tool with the Object ID. It will return the names and roles of the people involved in the item's creation.

**Q: Is it possible to see what is currently on display at the museum?**
Absolutely. The `get_objects_on_display` tool provides a paginated list of all objects currently featured in the physical galleries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cooper-hewitt](https://vinkius.com/mcp/cooper-hewitt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cooper Hewitt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cooper-hewitt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cooper Hewitt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cooper-hewitt": {
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
