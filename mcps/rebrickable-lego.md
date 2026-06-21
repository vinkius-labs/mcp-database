# Rebrickable LEGO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rebrickable-lego)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Explore the LEGO universe — search sets, parts, minifigs, themes and colors with full catalog data from any AI agent.

## Description
Connect to the **Rebrickable LEGO API** and explore the entire LEGO catalog through natural conversation.

### What you can do

- **Sets** — Search and browse LEGO sets by theme, year or part number with piece counts and images
- **Parts** — Explore the official LEGO parts catalog with part numbers, names and categories
- **Minifigures** — Discover minifigures with their set numbers, themes and images
- **Themes** — Browse all LEGO themes and sub-themes with set counts
- **Colors** — List all LEGO colors with their IDs, names and RGB values
- **Set Parts** — Get complete parts inventories for any LEGO set including spare parts

### How it works

1. Subscribe to this server
2. Enter your Rebrickable API Key
3. Start exploring LEGO data from Claude, Cursor, or any MCP-compatible client

No more navigating the Rebrickable website to find set details or parts inventories. Your AI acts as a dedicated LEGO archivist.

### Who is this for?

- **LEGO Fans** — discover sets by theme, find specific minifigures and explore the parts inventory
- **MOC Builders** — search for parts by number, check available colors and browse themes for inspiration
- **Collectors** — track sets by year, find specific editions and discover theme collections


## Available Tools
- **get_minifig**: g. "sw0001-1"). Returns the minifig name, theme, year, piece count and image URLs.

Get details for a specific LEGO minifigure
- **get_part**: g. "3001" for a 2x4 brick). Returns the part name, category, image URLs and available colors.

Get details for a specific LEGO part
- **get_part_colors**: Returns color IDs, color names and availability info. Useful for finding which colors a part is available in for MOC building.

Get available colors for a LEGO part
- **get_set**: g. "75192-1"). Returns the set name, year, theme, piece count, minifig count, image URLs and related info. Set numbers follow the format "NNNN-N" where NNNN is the set number and N is the variant.

Get details for a specific LEGO set
- **get_set_parts**: Each entry includes the part number, color ID, quantity and whether it's a spare part. Optionally include minifig parts. Use list_colors and list_parts to resolve color and part details.

Get the parts inventory for a LEGO set
- **get_theme**: Returns the theme name, parent theme (if sub-theme) and set count.

Get details for a specific LEGO theme
- **list_colors**: Useful for understanding color availability in sets and MOC building.

List all LEGO colors in the catalog
- **list_minifigs**: Returns minifig numbers, names, themes, year and image URLs. Optionally filter by part number. Use pagination with page and page_size (max 1000).

Search LEGO minifigures
- **list_parts**: Returns part numbers, names, categories and image URLs. Optionally filter by part number pattern. Use pagination with page and page_size (max 1000).

Search LEGO parts in the catalog
- **list_sets**: Optionally filter by theme ID, year, or part number. Returns set numbers, names, year, theme, piece count and image URLs. Use pagination with page and page_size (max 1000 per request).

Search LEGO sets in the Rebrickable catalog
- **list_themes**: g. Star Wars, City, Technic) and their sub-themes. Each theme includes its ID, name, parent theme ID (for sub-themes) and set count. Optionally filter by parent theme ID to get sub-themes of a specific theme.

List LEGO themes and sub-themes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebrickable LEGO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all LEGO Star Wars sets from 2024."

**🤖 AI Agent:**
> Found 15 Star Wars sets from 2024. Highlights include: '75375 Millennium Falcon' (921 pieces), '75367 Venator-Class Republic Attack Cruiser' (5374 pieces), and several UCS and polybag sets. Results include piece counts, themes and image URLs.

---

**👤 You:**
> "Show me the parts inventory for set 10497 (Galaxy Explorer)."

**🤖 AI Agent:**
> The Galaxy Explorer (10497-1) contains 235 parts across 42 unique pieces. Key parts include: 4x 2x4 bricks (part 3001), 6x 1x2 tiles, 2x windshield pieces, and various slope and plate elements. 2 spare parts are included.

---

**👤 You:**
> "What colors is LEGO part 3001 (2x4 brick) available in?"

**🤖 AI Agent:**
> Part 3001 (2x4 brick) is available in 55+ colors including: Black (0), White (1), Red (5), Blue (23), Green (10), Yellow (14), Dark Blue (140), Dark Green (137), Light Bluish Gray (86), Dark Red (59) and many specialty colors.


## ❓ FAQ

**Q: How do I get a Rebrickable API key?**
Visit [**rebrickable.com/api**](https://rebrickable.com/api/), sign in with your Rebrickable account, and your API key will be displayed on the page. Copy it — it's a long alphanumeric string.

**Q: Can I search for sets by theme?**
Yes! Use `list_sets` with `theme_id` to filter by theme. First use `list_themes` to find the theme ID (e.g. Star Wars = 170), then pass it to list_sets. You can also filter by year or part number.

**Q: Can I see the parts inventory for a set?**
Yes! Use `get_set_parts` with the set number (e.g. "75192-1" for the Millennium Falcon). Returns every part with its part number, color ID, quantity and whether it's a spare. Set inc_minifig_parts to true to include minifig parts.

**Q: How many results can I get at once?**
The API supports up to 1000 results per request. Use the `page_size` parameter (max 1000, default 100) and `page` for pagination. The total count and next/previous URLs are returned in each response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rebrickable-lego](https://vinkius.com/mcp/rebrickable-lego)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebrickable LEGO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rebrickable-lego` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebrickable LEGO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebrickable-lego": {
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
