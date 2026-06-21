# Trakt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trakt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track TV shows and movies — search titles, get ratings, discover trending content and manage your watchlist.

## Description
Connect to **Trakt** and explore the world's most popular TV and movie tracking platform through natural conversation.

### What you can do

- **Search** — Find movies, TV shows, episodes and people by title or name
- **Movie Details** — Get ratings, cast, crew, genres and related movies
- **Show Details** — Get seasons, episodes, cast, ratings and related shows
- **Trending** — See what's currently trending on Trakt in real-time
- **Popular** — Discover the most popular movies and shows
- **Calendar** — Get upcoming episode premieres and air dates

### How it works

1. Subscribe to this server
2. Enter your Trakt Client ID (free at trakt.tv/oauth/applications)
3. Start exploring TV and movie data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **TV & Movie Fans** — discover trending content, check ratings and find new shows to watch
- **Content Creators** — research cast info, ratings and related content for reviews
- **Recommendation Engines** — build watchlists and discover related content programmatically


## Available Tools
- **get_calendar**: Scope can be "my" (user's watched shows) or "all" (all shows). Returns episodes with air dates, times and show info.

Get upcoming episode calendar
- **get_collection**: Requires OAuth access token. Returns collected items with metadata and media info.

Get the authenticated user's collection
- **get_history**: Requires OAuth access token. Optionally filter by type and ID.

Get the authenticated user's watch history
- **get_movie**: Returns title, year, overview, runtime, rating, genres, languages, certification, trailer and poster URLs.

Get detailed info for a specific movie
- **get_movie_people**: Each person includes their name, Trakt ID, character name (for cast) and job title (for crew).

Get cast and crew for a specific movie
- **get_movie_ratings**: Returns total ratings, average score and the count of votes for each rating level.

Get ratings distribution for a specific movie
- **get_popular**: Popularity is based on overall engagement and activity. Returns paginated results.

Get the most popular movies or shows
- **get_related_movies**: Each related movie includes title, year, overview, rating and poster URL.

Get movies related to a specific movie
- **get_related_shows**: Each related show includes title, year, overview, rating and poster URL.

Get shows related to a specific TV show
- **get_show**: Returns title, year, overview, status, runtime, rating, genres, network, certification, trailer and poster URLs.

Get detailed info for a specific TV show
- **get_show_episodes**: Each episode includes episode number, title, overview, runtime, ratings and first aired date.

Get all episodes for a specific season of a TV show
- **get_show_people**: Get cast and crew for a TV show
- **get_show_ratings**: Returns total ratings, average score and vote counts per rating level.

Get ratings distribution for a TV show
- **get_show_seasons**: Each season includes season number, episode count, air date, rating and overview.

Get all seasons for a TV show
- **get_trending**: Trending is based on what users are actively watching and checking in. Returns items with viewer counts.

Get currently trending movies or shows
- **get_watched**: Requires OAuth access token. Returns items with play counts and last watched timestamps.

Get the authenticated user's watched history
- **get_watchlist**: Requires an OAuth access token. Returns movies and/or shows the user has added to their watchlist.

Get the authenticated user's watchlist
- **search**: Returns results with titles, years, ratings, genres, IDs and synopsis. Use type parameter to narrow results: "movie", "show", "episode", "person" or "list".

Search for movies, shows, episodes, people or lists on Trakt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trakt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What movies are trending right now?"

**🤖 AI Agent:**
> Top trending movies: 1. Dune: Part Two (3.2K viewers) — 2. Oppenheimer (2.8K) — 3. Deadpool & Wolverine (2.1K) — 4. The Batman (1.9K) — 5. Poor Things (1.5K). All with viewer counts and ratings.

---

**👤 You:**
> "Show me info about Breaking Bad."

**🤖 AI Agent:**
> Breaking Bad (2008-2013) — Rating: 9.5/10 from 125K votes. Genres: Drama, Crime, Thriller. Network: AMC. 5 seasons, 62 episodes. Overview: A high school chemistry teacher diagnosed with terminal cancer turns to manufacturing meth to secure his family's future.

---

**👤 You:**
> "Who directed The Matrix and who starred in it?"

**🤖 AI Agent:**
> The Matrix (1999) — Directors: Lana Wachowski, Lilly Wachowski. Cast: Keanu Reeves (Neo), Laurence Fishburne (Morpheus), Carrie-Anne Moss (Trinity), Hugo Weaving (Agent Smith), Joe Pantoliano (Cypher).


## ❓ FAQ

**Q: How do I get a Trakt Client ID?**
Sign up for a free Trakt account at [**trakt.tv**](https://trakt.tv), go to [**OAuth Applications**](https://trakt.tv/oauth/applications), click 'Create an Application' and fill in the details. Your Client ID is displayed immediately.

**Q: Can I use IDs from IMDb or TVDB?**
Yes! Trakt accepts Trakt IDs, URL slugs (e.g. 'the-matrix'), IMDb IDs (e.g. 'tt0133093') and TMDB IDs for movies. For shows it accepts Trakt IDs, slugs, TVDB IDs and TMDB IDs.

**Q: What's the difference between trending and popular?**
Trending shows what users are actively watching RIGHT NOW (real-time). Popular shows have the highest overall engagement over time. Trending is more dynamic and changes frequently.

**Q: Can I sync my watchlist and history?**
Yes! Use get_watchlist, get_watched, get_collection and get_history with OAuth authentication. These endpoints require an access token in addition to your Client ID. Visit trakt.tv/oauth/applications to set up OAuth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trakt](https://vinkius.com/mcp/trakt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trakt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trakt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trakt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trakt": {
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
