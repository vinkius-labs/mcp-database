# OMDb API MCP Server

Search movies & TV shows, get ratings, cast, plot details, and IMDb data via the Open Movie Database API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/omdb-api)

## Overview
**Category:** data-analytics
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **OMDb API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omdb-api](https://vinkius.com/mcp/omdb-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
