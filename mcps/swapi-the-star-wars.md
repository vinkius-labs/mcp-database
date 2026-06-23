# SWAPI - The Star Wars MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swapi-the-star-wars)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Explore the Star Wars universe — query people, planets, films, and starships directly from the Star Wars API.

## Description
Access the comprehensive **Star Wars API (SWAPI)** through your AI agent and dive deep into the lore of the galaxy far, far away.

### What you can do

- **Characters & People** — Search for iconic characters like Luke Skywalker or Darth Vader and get their physical traits and history.
- **Planets & Moons** — Retrieve data on climates, terrain, and populations for worlds like Tatooine or Coruscant.
- **Starships & Vehicles** — Get technical specifications for the Millennium Falcon, X-wings, and Imperial Star Destroyers.
- **Films & Species** — List all movies in the saga or explore the diverse biological species inhabiting the galaxy.
- **Deep Linking** — Use specific resource URLs to navigate between related data points like a character's homeworld or the films they appeared in.

### How it works

1. Subscribe to this server
2. No API key is required as SWAPI is a public resource
3. Start exploring the galaxy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly test API structures or fetch Star Wars placeholder data for applications.
- **Fans & Writers** — verify facts about characters, ships, and planets for creative projects.
- **Data Enthusiasts** — analyze the relationships between different entities in the Star Wars universe.


## Available Tools (8)
- **get_resource_by_url**: g., from a homeworld, films, or species attribute).

Get a specific SWAPI resource by its URL
- **get_root**: Get SWAPI root resources
- **list_films**: Use the search parameter to filter by title.

List or search Star Wars films
- **list_people**: Use the search parameter to filter by name.

List or search Star Wars people/characters
- **list_planets**: Use the search parameter to filter by name.

List or search Star Wars planets
- **list_species**: Use the search parameter to filter by name.

List or search Star Wars species
- **list_starships**: Use the search parameter to filter by name or model.

List or search Star Wars starships
- **list_vehicles**: Use the search parameter to filter by name or model.

List or search Star Wars vehicles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SWAPI - The Star Wars** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the character 'Darth Vader' and tell me his height."

**🤖 AI Agent:**
> I found Darth Vader. According to the records, he is 202 cm tall and weighs 136 kg.

---

**👤 You:**
> "List all the planets in the Star Wars universe."

**🤖 AI Agent:**
> Fetching planets... I've found several worlds including Tatooine, Alderaan, Yavin IV, and Hoth. Would you like details on a specific one?

---

**👤 You:**
> "What are the technical specifications of the Millennium Falcon?"

**🤖 AI Agent:**
> The Millennium Falcon (model YT-1300 light freighter) has a max atmosphering speed of 1050 km/h, a hyperdrive rating of 0.5, and can carry up to 6 passengers.


## ❓ FAQ

**Q: How can I find a specific character by their name?**
You can use the `list_people` tool and provide the name in the `search` parameter. The agent will return all matching characters from the Star Wars universe.

**Q: How do I get more details about a URL found in a result (like a homeworld)?**
Use the `get_resource_by_url` tool. Simply pass the full URL (e.g., https://swapi.dev/api/planets/1/) to fetch the complete metadata for that specific resource.

**Q: Can I search for starships using their model name instead of their common name?**
Yes! The `list_starships` tool allows searching by both name and model. Just enter the model string into the `search` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swapi-the-star-wars](https://vinkius.com/mcp/swapi-the-star-wars)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SWAPI - The Star Wars** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swapi-the-star-wars` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SWAPI - The Star Wars** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swapi-the-star-wars": {
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
