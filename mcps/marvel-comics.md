# Marvel Comics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marvel-comics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Explore the Marvel universe — search characters, comics, series, events and creators with full metadata from any AI agent.

## Description
Connect to the **Marvel Comics API** and explore the entire Marvel universe through natural conversation.

### What you can do

- **Characters** — Search and discover Marvel characters (Spider-Man, Iron Man, X-Men, Avengers) with bios and images
- **Comics** — Find specific comics by title or browse by character, with issue numbers, formats and cover dates
- **Series** — Explore comic series from classic runs to modern limited series with start/end years
- **Events** — Discover major crossover events (Civil War, Secret Wars, Infinity War) with involved comics and characters
- **Creators** — Find writers, artists, editors and colorists who brought Marvel stories to life

### How it works

1. Subscribe to this server
2. Enter your Marvel Public and Private API Keys
3. Start exploring the Marvel universe from Claude, Cursor, or any MCP-compatible client

No more navigating the Marvel website or wikis to find character bios or comic details. Your AI acts as a dedicated Marvel archivist.

### Who is this for?

- **Comic Fans** — discover character backstories, find specific comics and explore major story arcs
- **Collectors** — search for comics by character, series or title to track down specific issues
- **Researchers** — explore Marvel's publication history, creator credits and event timelines


## Available Tools (10)
- **get_character**: Returns the character name, description, thumbnail image URL, comics appearances, series, events and related creators. Use list_characters to find character IDs by name first.

Get a Marvel character by ID
- **get_comic**: Returns the comic title, description, issue number, format, publication date, prices, creators and characters. Use list_comics to find comic IDs first.

Get a Marvel comic by ID
- **get_creator**: ) by their numeric ID. Returns their full name, role, comics worked on, series and events. Use list_creators to find creator IDs by name first.

Get a Marvel creator by ID
- **get_event**: g. "Civil War", "Secret Wars", "Infinity War"). Returns the event title, description, start/end dates, number of comics/series/characters involved and thumbnail.

Get a Marvel event by ID
- **get_series**: Returns the series title, description, start/end years, number of issues, thumbnail and related content.

Get a Marvel series by ID
- **list_characters**: Returns character IDs, names, descriptions and thumbnail images. Useful for discovering character IDs to use with get_character, get_comics (by character) and other tools. Optionally set limit (max 100) and offset for pagination.

Search Marvel characters by name
- **list_comics**: Returns comic titles, issue numbers, formats, publication dates and cover images. Optionally filter by a specific character using their ID. Set limit (max 100) and offset for pagination.

Search Marvel comics by title or character
- **list_creators**: ) by first or last name prefix. Returns creator IDs, full names, thumbnails and their primary roles. Useful for discovering who worked on specific comics. Set limit (max 100) for pagination.

Search Marvel creators by name
- **list_events**: Returns event titles, descriptions, start/end dates and number of involved comics/series. Useful for discovering major story arcs. Set limit (max 100) for pagination.

Search Marvel events by name or character
- **list_series**: Returns series titles, start/end years, issue counts and thumbnails. Useful for finding ongoing series and limited runs. Set limit (max 100) for pagination.

Search Marvel series by title or character


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marvel Comics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all characters whose names start with 'Iron'."

**🤖 AI Agent:**
> Found 5 characters: Iron Man (Tony Stark) - Genius billionaire inventor in a powered suit of armor, Iron Fist (Danny Rand) - Martial artist with mystical chi-powered fist, Iron Patriot, Ironheart (Riri Williams) - Teen genius who built her own armor, and Iron Lad (young Kang variant).

---

**👤 You:**
> "What comics feature the X-Men?"

**🤖 AI Agent:**
> I found 200+ comics featuring the X-Men character (ID 1009726). Recent titles include 'X-Men #25' (2024), 'X-Men: Red', 'Uncanny X-Men', 'New Mutants' and 'X-Factor'. Results include issue numbers, formats (comic, hardcover, trade paperback), cover dates and prices.

---

**👤 You:**
> "Tell me about the Civil War event."

**🤖 AI Agent:**
> Civil War (2006-2007) was a major Marvel crossover event written by Mark Millar with art by Steve McNiven. The conflict divided heroes over the Superhuman Registration Act, pitting Iron Man against Captain America. The event spanned 7 main issues and over 100 tie-in comics across multiple series.


## ❓ FAQ

**Q: How do I get Marvel API keys?**
Visit [**developer.marvel.com/account**](https://developer.marvel.com/account), sign in with a Marvel or social account, and you'll immediately see your Public and Private keys. Both are required for authentication.

**Q: Can I search for characters by name?**
Yes! Use `list_characters` with `name_starts_with` to search. For example, 'Spider' returns Spider-Man (Peter Parker), Spider-Man (Miles Morales), Spider-Gwen and more. Each result includes the character ID for use with other tools.

**Q: Can I find comics for a specific character?**
Yes! Use `list_comics` with `character_id`. First find the character ID with `list_characters`, then pass it to `list_comics` to get all their comic appearances with issue numbers, titles and cover dates.

**Q: How many results can I get at once?**
The API supports up to 100 results per request. Use the `limit` parameter (1-100, default 20) and `offset` for pagination. The total count is returned in each response so you know how many pages exist.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marvel-comics](https://vinkius.com/mcp/marvel-comics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marvel Comics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marvel-comics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marvel Comics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marvel-comics": {
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
