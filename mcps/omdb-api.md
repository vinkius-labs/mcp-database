# OMDb API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omdb-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search movies & TV shows, get ratings, cast, plot details, and IMDb data via the Open Movie Database API.

## Description
Connect the **OMDb API (Open Movie Database)** to any AI agent and access comprehensive movie and TV show data including IMDb ratings, Rotten Tomatoes scores, full cast & crew, plot summaries, box office figures, and awards through natural conversation.

### What you can do

- **Search Movies & Series** — Find any movie or TV show by title keyword with results showing IMDb ID, type, year, and poster references
- **Get by IMDb ID** — Retrieve complete details for any title using its unique IMDb ID (most accurate method, no title ambiguity)
- **Get by Title** — Look up any movie or series by its exact title with optional filters for type and release year
- **Full Plot Synopses** — Access both short and full-length plot summaries for deep understanding of any film or series
- **Multi-Source Ratings** — Get ratings from IMDb, Rotten Tomatoes, and Metacritic all in one call to compare critical consensus
- **Search by Type** — Filter searches specifically for movies, TV series, or episodes to narrow results precisely
- **Episode Details** — Get information about specific TV episodes including air date, synopsis, director, and writer
- **Batch Lookup** — Retrieve details for multiple titles at once using comma-separated IMDb IDs — perfect for franchise comparisons
- **Box Office Data** — Access theatrical box office gross figures for movies
- **Production & Awards** — Get studio information, award details, and content ratings (PG, PG-13, R, etc.)

### How it works

1. Subscribe to this server
2. Enter your OMDb API Key (free, 1,000 requests/day)
3. Start searching movies, getting ratings, and exploring film data from Claude, Cursor, or any MCP-compatible client

The OMDb API is a simple, lightweight alternative to larger databases — perfect for quick lookups, rating checks, and IMDb cross-referencing without complex setup.

### Who is this for?

- **Movie Enthusiasts** — quickly look up ratings, plot summaries, and cast details without switching between IMDb, Rotten Tomatoes, and Wikipedia
- **TV Show Fans** — search for series, find episode information, and track show metadata across seasons
- **Content Creators & Reviewers** — access ratings from multiple sources (IMDb, RT, Metacritic) in one call to create comparison content
- **Data Analysts** — batch-process multiple IMDb IDs at once for franchise analysis or comparative studies


## Available Tools (12)
- **get_by_imdb_id**: g., "tt0468569" for The Dark Knight). Returns: Title, Year, Rated (content rating), Released (date), Runtime, Genre, Director, Writer, Actors, Plot, Language, Country, Awards, Ratings (IMDb, Rotten Tomatoes, Metacritic), Metascore, imdbRating, imdbVotes, imdbID, Type (movie/series/episode), DVD release date, BoxOffice gross, Production studio, and Website. Use this when you have an IMDb ID and need complete movie/series information. This is the most accurate method — IMDb IDs are unique and unambiguous. Optional plot parameter: "short" (brief synopsis) or "full" (complete plot summary).

Get complete details for a movie or TV series using its IMDb ID
- **get_by_title**: Returns the same fields as get_by_imdb_id: Title, Year, Rated, Runtime, Genre, Director, Writer, Actors, Plot, Ratings (IMDb, Rotten Tomatoes, Metacritic), BoxOffice, Production studio, etc. Use this when you know the title but not the IMDb ID. IMPORTANT: If multiple items share the same title, the API may return the first match or an error. To narrow results, use the optional type filter (movie/series/episode) and year filter. For more precise matching, prefer get_by_imdb_id when available.

Get details for a movie or TV series by its exact title
- **get_episode**: Returns: Title (episode name), Year (air year), Released (air date), Runtime, Genre, Director, Writer, Actors, Plot (episode synopsis), Language, Country, Ratings, imdbRating, imdbVotes, imdbID, and Type (episode). Use this after finding an episode via search_episodes to get its full details. The IMDb ID is required — get it from search results or from a TV series season/episode listing.

Get details for a specific TV episode using its IMDb ID
- **get_full_by_imdb_id**: This is the same as get_by_imdb_id but always uses plot="full" for the most comprehensive synopsis. Returns: Title, Year, Rated, Released, Runtime, Genre, Director, Writer, Actors, full Plot, Language, Country, Awards, Ratings (IMDb, Rotten Tomatoes, Metacritic), Metascore, imdbRating, imdbVotes, imdbID, Type, DVD release date, BoxOffice gross, Production studio, and Website. Using IMDb ID is the most accurate method — IDs are unique and unambiguous unlike titles which can have duplicates. The full plot provides deeper synopsis detail compared to the short version.

Get the most detailed information for a movie or series using its IMDb ID
- **get_full_by_title**: This is the same as get_by_title but always uses plot="full" for the most comprehensive synopsis. Returns: Title, Year, Rated, Released, Runtime, Genre, Director, Writer, Actors, full Plot, Language, Country, Awards, Ratings (IMDb, Rotten Tomatoes, Metacritic), Metascore, imdbRating, imdbVotes, imdbID, Type, DVD release date, BoxOffice gross, Production studio, and Website. Use this when users want the complete plot summary and all metadata for a specific title. The full plot can be significantly longer than the short version, providing deeper synopsis detail.

Get the most detailed information for a movie or series by title
- **get_multiple_by_id**: Each ID is fetched individually and results are combined into one response. If any ID fails, it will be returned with an error message while others still succeed. Use this when comparing multiple films, getting info for a franchise, or batch-processing a list of IMDb IDs. Format: comma-separated IMDb IDs without spaces (e.g., "tt0468569,tt1375666,tt0816692"). Each result includes: Title, Year, Rated, Runtime, Genre, Director, Actors, Plot (short), Ratings, imdbRating, imdbVotes, Type, BoxOffice, Production, and more.

Get details for multiple movies/series at once using their IMDb IDs
- **get_ratings**: Also returns: Title, Year, Type, imdbRating, imdbVotes, and Metascore as individual fields. Use this when users ask "what is the rating of...", "how is X rated?", or want to compare scores across platforms. You can search by title (first parameter) or by IMDb ID (set use_imdb_id=true for the second parameter). Note: Not all titles have ratings from all three sources — some may be missing.

Get all available ratings (IMDb, Rotten Tomatoes, Metacritic) for a movie or series
- **get_short_plot**: The short plot provides a concise synopsis — ideal for quick identification or brief descriptions. Returns: Title, Year, Rated, Runtime, Genre, Director, Actors, short Plot, Ratings, and other metadata. Use this when users want a quick summary without the lengthy full plot. For the complete synopsis, use get_full_by_title or get_full_by_imdb_id instead.

Get a brief plot summary for a movie or series by title
- **search**: Returns a paginated list of matching titles. Each result includes: Title, Year, IMDb ID, Type (movie/series/episode), and Poster URL. Results are paginated (10 per page); use the page parameter to get more results (pages 1-100). Use this when users ask to "find movies about..." or "search for..." a topic. Optional filters: type (movie/series/episode) and year (YYYY format). Note: Search results are brief — use get_by_imdb_id or get_by_title with the returned IMDb ID for full details.

Search for movies, TV series, or episodes by title keyword
- **search_episodes**: Returns a paginated list of matching episode titles. Each result includes: Title, Year, IMDb ID, Type (always "episode"), and Poster URL. Use this when users want to find specific TV episodes by title or keyword. Episode titles often include the series name followed by the episode name. Results are paginated (10 per page); use the page parameter to navigate results.

Search for TV episodes only (excludes movies and full series)
- **search_movies**: Returns a paginated list of matching movie titles. Each result includes: Title, Year, IMDb ID, Type (always "movie"), and Poster URL. Use this when users specifically want to find movies (not TV shows) by keyword. Results are paginated (10 per page); use the page parameter to navigate results. Optional year filter narrows results to a specific release year.

Search for movies only (excludes TV series and episodes)
- **search_series**: Returns a paginated list of matching series titles. Each result includes: Title, Year (or year range like "2008-2013"), IMDb ID, Type (always "series"), and Poster URL. Use this when users specifically want to find TV shows (not movies) by keyword. Results are paginated (10 per page); use the page parameter to navigate results. Optional year filter narrows results to series that started in a specific year.

Search for TV series only (excludes movies and episodes)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OMDb API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the ratings for The Dark Knight?"

**🤖 AI Agent:**
> The Dark Knight (2008) ratings: ⭐ IMDb: 9.0/10 (2.8M votes) | 🍅 Rotten Tomatoes: 94% | 📊 Metacritic: 84/100. Rated PG-13. Directed by Christopher Nolan, starring Christian Bale and Heath Ledger. Box Office: $534,858,444. A critically acclaimed superhero film widely considered one of the best of all time.

---

**👤 You:**
> "Search for movies directed by Christopher Nolan with Interstellar in the title."

**🤖 AI Agent:**
> Found: Interstellar (2014) — ⭐ 8.7/10 on IMDb. Runtime: 169 min. Genre: Adventure, Drama, Sci-Fi. Cast: Matthew McConaughey, Anne Hathaway, Jessica Chastain. Director: Christopher Nolan. Plot: A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival as Earth becomes uninhabitable. Box Office: $701,729,206. Production: Paramount Pictures.

---

**👤 You:**
> "Compare the Lord of the Rings trilogy movies: tt0120737, tt0167261, tt0167260"

**🤖 AI Agent:**
> LotR trilogy comparison:
1) The Fellowship of the Ring (2001) ⭐ 8.9 — Runtime: 178 min | Box Office: $897.7M
2) The Two Towers (2002) ⭐ 8.8 — Runtime: 179 min | Box Office: $947.9M
3) The Return of the King (2003) ⭐ 9.0 — Runtime: 201 min | Box Office: $1.146B
All directed by Peter Jackson. Return of the King won 11 Academy Awards including Best Picture.


## ❓ FAQ

**Q: What's the difference between searching by title vs. using an IMDb ID?**
Using an IMDb ID (e.g., `tt0468569`) is the most accurate method because IDs are unique — there's never ambiguity between different films with the same name. Searching by title can return errors if multiple films share the same title (e.g., "King Kong" has multiple versions). If you know the IMDb ID from a link or another source, always prefer `get_by_imdb_id`. Use `get_by_title` when you only know the film name.

**Q: Can I get ratings from multiple sources (IMDb, Rotten Tomatoes, Metacritic) at once?**
Yes! Use the `get_ratings` tool with either a movie title or IMDb ID. It returns all available ratings from IMDb (out of 10), Rotten Tomatoes (percentage), and Metacritic (out of 100) in a single call. Not all titles have all three ratings — newer or less popular films may only have IMDb data. The tool also returns the IMDb vote count and Metascore as separate fields.

**Q: Can I look up details for multiple movies at the same time?**
Yes! Use the `get_multiple_by_id` tool with comma-separated IMDb IDs (e.g., `tt0468569,tt1375666,tt0816692` for the Dark Knight trilogy). It fetches details for each ID and returns them combined in one response. If any ID fails, it shows an error for that specific ID while still returning results for the others. This is ideal for franchise comparisons or batch analysis.

**Q: What's the difference between short and full plot summaries?**
The short plot provides a concise 1-2 paragraph summary — ideal for quick identification or brief descriptions. The full plot offers a much more detailed synopsis with deeper plot points, character arcs, and story resolution. Use short for quick lookups (`get_by_title`, `get_short_plot`) and full when users want comprehensive understanding (`get_full_by_title`, `get_full_by_imdb_id`).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omdb-api](https://vinkius.com/mcp/omdb-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OMDb API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `omdb-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OMDb API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omdb-api": {
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
