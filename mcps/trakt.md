# Trakt MCP Server

Track TV shows and movies — search titles, get ratings, discover trending content and manage your watchlist.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/trakt)

## Overview
**Category:** productivity
**Tools Count:** 18

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


## Installation & Usage

To install and use the **Trakt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trakt](https://vinkius.com/mcp/trakt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
