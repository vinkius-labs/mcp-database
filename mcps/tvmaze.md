# TVMaze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tvmaze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tvmaze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tvmaze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search TV shows, get episode guides, browse schedules, discover cast and crew — no API key required.

## Description
Connect to **TVMaze** and explore the world's TV database through natural conversation — no API key needed.

### What you can do

- **Show Search** — Search for TV shows by title with fuzzy matching and typo tolerance
- **Show Details** — Get complete info including genres, network, ratings, status and external IDs (IMDb, TheTVDB)
- **Episode Guides** — Browse all episodes with season/episode numbers, air dates and summaries
- **Cast & Crew** — Discover who starred in a show and find directors, writers and producers
- **TV Schedule** — Check what's airing today or on any date, filtered by country
- **People Search** — Find actors and crew members with their full filmography
- **Show Images** — Access posters, banners and background images for any show

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore TV data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free with CC BY-SA license.

### Who is this for?

- **TV Fans** — discover new shows, check episode guides and find out who starred in their favorites
- **Binge Watchers** — browse episode lists, check season counts and find out when shows premiered
- **Researchers** — access TV schedule data, explore crew credits and track show statuses


## Available Tools
- **get_episode**: Returns the episode name, season and number, air date, summary, runtime, image URL and show link.

Get detailed info for a specific episode by ID
- **get_full_schedule**: Returns all known future episodes across all shows and networks. This is a large response (multiple MB). Optionally filter by country code.

Get the full future TV schedule
- **get_person**: ) by their numeric ID. Returns the person's name, birthday, birthplace, gender, photo, bio and external IDs (IMDb, Wikipedia, TVRage).

Get detailed info for a specific person
- **get_person_cast_credits**: Each credit includes the show name, character name, episode count and whether the role was main or recurring.

Get all cast credits for a person
- **get_schedule**: Each entry includes the show name, episode name, airtime, network and episode info. Optionally set country (ISO 3166-1 alpha-2 code, e.g. "US", "GB", "BR") and date (YYYY-MM-DD, default today).

Get TV schedule for a specific date and country
- **get_show**: Returns the show name, genres, network, premiered date, ended date, rating, image URL, summary, runtime, status (running, ended, in development) and external IDs (IMDb, TheTVDB, TVRage).

Get detailed info for a specific TV show by ID
- **get_show_cast**: Each cast member includes the person's name, character name and a link to their photo. Useful for discovering who starred in a show.

Get the cast for a TV show
- **get_show_crew**: ) for a TV show. Each crew member includes their name, role type and credit type. Useful for finding directors, creators and key production staff.

Get the crew for a TV show
- **get_show_episodes**: Each episode includes the season and episode number, air date, name, summary, runtime and image URL. By default, special episodes are excluded; set specials=true to include them.

Get all episodes for a TV show
- **get_show_images**: Each image includes its type, resolution, and URL.

Get images for a TV show
- **get_show_seasons**: Each season includes its number, name, episode order, premiere date, network and image URL.

Get all seasons for a TV show
- **get_shows**: Returns only show IDs. Use get_show for details on specific shows.

Browse all TV shows in the database
- **search_people**: Uses fuzzy matching. Returns multiple results with person names, photos and their notable shows.

Search for actors and crew by name
- **search_shows**: Uses fuzzy matching with tolerance for typos. Returns multiple results ranked by relevance. Each result includes the show's name, genres, network, premiered year, rating, image URL and summary. Use single_search for exact single match.

Search for TV shows by name
- **single_search**: Returns exactly one result or none. Includes embedded details like episodes, cast and network info. Use this when you want the best match for a specific show name.

Search for a single TV show with full details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TVMaze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Breaking Bad' and show me details."

**🤖 AI Agent:**
> Breaking Bad is a drama/crime/thriller series that aired on AMC from 2008 to 2013. Created by Vince Gilligan, it stars Bryan Cranston as Walter White. 5 seasons, 62 episodes. Rating: 9.5/10. Status: Ended. Network: AMC.

---

**👤 You:**
> "Show me the full cast of The Office."

**🤖 AI Agent:**
> Main cast of The Office: Steve Carell as Michael Scott, John Krasinski as Jim Halpert, Jenna Fischer as Pam Beesly, Rainn Wilson as Dwight Schrute, B.J. Novak as Ryan Howard, Mindy Kaling as Kelly Kapoor, Ed Helms as Andy Bernard and 15 more.

---

**👤 You:**
> "What's on TV tonight in the US?"

**🤖 AI Agent:**
> Tonight's US TV schedule includes: 'NCIS' (CBS, 8:00 PM, S21E10 'The Core'), 'The Voice' (NBC, 8:00 PM, live playoffs), 'Abbott Elementary' (ABC, 9:00 PM, S4E05), 'FBI' (CBS, 9:00 PM), and 20+ more shows across major networks.


## Installation & Usage

To install and use the **TVMaze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tvmaze](https://vinkius.com/mcp/tvmaze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
