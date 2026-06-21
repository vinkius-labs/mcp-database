# The Movie Database (TMDb) MCP Server

Search movies, TV shows, people, get details, cast, trailers, and discover content via TMDb API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/the-movie-database-tmdb)

## Overview
**Category:** knowledge-management
**Tools Count:** 15

## Description
Connect **The Movie Database (TMDb)** to any AI agent and unlock the world's most comprehensive movie and TV show database through natural conversation. TMDb is the same database used by major streaming platforms, media players, and entertainment apps worldwide.

### What you can do

- **Movie Search** — Search any movie by title, keyword, or phrase with release dates, ratings, overviews, and poster images
- **TV Show Search** — Find TV shows and series with season counts, episode information, network details, and air dates
- **Unified Multi-Search** — Search movies, TV shows, and people simultaneously for broad entertainment queries
- **Complete Movie Details** — Get full movie metadata including budget, revenue, runtime, genres, production studios, taglines, and IMDb cross-references
- **Cast & Crew Information** — Retrieve complete cast lists with actor characters and crew details (directors, writers, producers, cinematographers)
- **Trailers & Videos** — Access official trailers, teasers, behind-the-scenes clips, and promotional videos (YouTube links)
- **Popular & Top Rated** — Browse currently popular movies/TV shows and all-time highest-rated content
- **Trending Content** — See what is trending today or this week across movies, TV shows, and people
- **Advanced Movie Discovery** — Filter movies by genre, year, minimum rating, production studio (e.g., Warner Bros., Marvel), and sort by popularity, rating, or revenue
- **Movie Recommendations** — Get similar movie suggestions based on a specific film using TMDb's recommendation algorithm
- **Person Profiles** — Search for actors, directors, and crew with biographies, filmographies, and combined credits
- **External ID Lookup** — Convert IMDb IDs (tt0111161), TVDb IDs, and other external identifiers to TMDb entries
- **Genre Reference** — Access the complete genre database with IDs for advanced filtering

### How it works

1. Subscribe to this server
2. Enter your TMDb API Key (v3 auth)
3. Start exploring movies, TV shows, cast info, and trailers from Claude, Cursor, or any MCP-compatible client

Your AI acts as a personal entertainment database assistant — no more switching between IMDb, Letterboxd, and streaming apps. Get instant answers about any movie or TV show.

### Who is this for?

- **Movie Buffs & Cinephiles** — instantly search filmographies, find cast details, discover similar movies, and explore trending films without opening multiple apps
- **TV Show Fans** — look up series information, season/episode counts, airing dates, and find what shows are popular or top-rated right now
- **Content Creators & Reviewers** — quickly access movie metadata, trailers, poster images, and cast information for video essays, reviews, and recommendations
- **Casual Viewers** — ask "what should I watch tonight?" and get personalized recommendations based on trending, top-rated, or genre-filtered results


## Available Tools
- **get_movie_credits**: Returns two arrays: "cast" (actors with their characters, order, and profile images) and "crew" (directors, producers, writers, cinematographers, editors, composers, etc. with their jobs and departments). Use this when users ask "who starred in...", "who directed...", or want the full cast list of a movie. The movieId is the TMDb ID from search results. Cast includes: actor name, character name, order (billing order), profile image path. Crew includes: name, job title (Director, Producer, Screenplay, etc.), department.

Get complete cast and crew information for a specific movie
- **popular_tv**: Popularity is based on user activity, view counts, and trending data. Each TV show includes: name, first air date, overview, poster path, vote average, vote count, genre IDs, number of seasons, number of episodes, origin country, and TMDb ID. Use this when users ask "what TV shows are popular?", "what should I watch?", or want series recommendations. Optional: page for pagination and language for localized titles and descriptions.

Get a list of currently popular TV shows on TMDb
- **find_by_external_id**: The externalSource parameter must be one of: "imdb_id", "tvdb_id", "freebase_mid", "freebase_id", "tvrage_id", "wikidata_id". Returns matching movies, TV shows, and/or people from TMDb that have this external ID. Use this when you have an IMDb ID (like "tt0111161" for Shawshank Redemption) and want to find the corresponding TMDb entry. Common use case: converting IMDb IDs to TMDb IDs for use with other tools. IMDb IDs for movies start with "tt" followed by numbers (e.g., "tt0137523" for Fight Club). Results include all matching items across movies, TV, and people categories.

Find movies, TV shows, or people using external IDs (IMDb, TVDb, etc)
- **discover_movies**: Find movies matching very specific criteria. Available filters: genre (genre IDs, comma-separated for OR), year, sortBy (popularity, rating, revenue, release date), vote_average.gte (minimum rating), with_companies (studio IDs, comma-separated), with_keywords (keyword IDs), primary_release_date.gte/lte (date range YYYY-MM-DD). Sort options: popularity.desc, popularity.asc, release_date.desc, release_date.asc, vote_average.desc, vote_average.asc, revenue.desc, revenue.asc, title.asc, title.desc. Use this for complex queries like "action movies from 2024 with rating above 7", "Warner Bros movies from the last year", or "horror movies sorted by rating". Genre IDs can be obtained from the get_genres tool. Company ID 17 = Warner Bros, 420 = Marvel Studios, 33 = Universal, etc.

Discover movies with advanced filtering by genre, year, rating, studio, and more
- **get_genres**: Each genre includes: id (numeric ID used for filtering in other tools) and name (localized genre name). Use this to get genre IDs needed for the discover_movies tool or to answer questions about available genres. Common movie genres: 28=Action, 12=Adventure, 16=Animation, 35=Comedy, 80=Crime, 18=Drama, 14=Fantasy, 27=Horror, 878=Science Fiction, 53=Thriller, 10749=Romance. The type parameter must be "movie" or "tv". Optional language parameter returns localized genre names.

Get the complete list of movie or TV show genres with their IDs
- **get_movie**: Returns: title, overview, runtime, release date, budget, revenue, vote average, vote count, genres, production companies, production countries, spoken languages, status, tagline, homepage, IMDb ID, poster/backdrop image paths, and collection information (if part of a franchise). Use this after a search to get full details about a specific movie. The movieId parameter is the TMDb ID (integer) returned by search_movies or other movie list tools. Optional language parameter returns localized title and overview if available.

Get complete details for a specific movie by its TMDb ID
- **get_movie_recommendations**: TMDb uses an algorithm that considers genre, keywords, cast, crew, and user rating patterns to suggest similar movies that fans of the original might enjoy. Each recommendation includes: title, release date, overview, poster path, vote average, vote count, and TMDb ID. Use this when users ask "if I liked X, what should I watch?", "movies similar to...", or "recommendations for...". The movieId is the TMDb ID of the reference movie. Results are paginated; use the page parameter to get more recommendations.

Get movie recommendations based on a specific movie (similar titles)
- **get_movie_videos**: Each video result includes: video key (YouTube ID), site (YouTube), type (Trailer, Teaser, Clip, Behind the Scenes, etc.), name, size (resolution), official status, and publish date. Use this when users want to watch trailers, find official promotional videos, or access movie video content. YouTube videos can be viewed at: https://www.youtube.com/watch?v={key}. The movieId is the TMDb movie ID.

Get trailers, teasers, clips, and behind-the-scenes videos for a movie
- **popular_movies**: Each movie includes: title, release date, overview, poster path, vote average, vote count, genre IDs, and TMDb ID. Use this when users ask "what movies are popular now?", "what is trending?", or want movie recommendations. Results are updated regularly based on TMDb user activity. Optional: page for pagination, region (ISO 3166-1 country code like "US", "BR") for country-specific popularity, and language for localized titles and descriptions.

Get a list of currently popular movies on TMDb
- **search_movies**: Returns movie titles, release dates, overview descriptions, poster images, vote averages, and TMDb IDs. Use this when users ask to find movies by title, search for films about a topic, or look up movies from a specific year. The query parameter is required and should be the movie title or search term. Optional parameters: year (YYYY format) to filter by release year, page for pagination (1-500), and language (ISO 639-1 code like "pt-BR", "en-US", "es") to get results in a specific language. Example: query="The Matrix", year="1999" returns the 1999 sci-fi classic.

Search for movies by title, keyword, or phrase in the TMDb database
- **search_multi**: Returns results from all three categories with a media_type field indicating the type ("movie", "tv", or "person"). Use this when users provide a general search term and you want to return all relevant results across content types. Ideal for broad queries like "Christopher Nolan" (returns movies directed by him + person profile) or "Star Wars" (returns movies + TV series). The query parameter is required. Optional: page for pagination and language for localized results.

Search movies, TV shows, and people simultaneously in the TMDb database
- **search_tv**: Returns TV show names, first air dates, episode counts, overview descriptions, poster images, vote averages, and TMDb IDs. Use this when users ask to find TV series, look up shows by title, or search for programs about a specific topic. The query parameter is required. Optional: year to filter by first air date year, page for pagination, and language for localized results. Example: query="Breaking Bad" returns the critically acclaimed drama series.

Search for TV shows by title or keyword in the TMDb database
- **top_rated_movies**: These are the critically acclaimed films with the best user ratings. Each movie includes: title, release date, overview, vote average, vote count, poster path, genre IDs, and TMDb ID. Use this when users ask for "best movies ever", "top rated films", "highest rated movies", or want quality recommendations. This list includes classics like The Shawshank Redemption, The Godfather, and other critically acclaimed films. Optional: page for pagination and language for localized results.

Get a list of the highest-rated movies of all time on TMDb
- **top_rated_tv**: These are the most critically acclaimed series with the best user ratings. Each TV show includes: name, first air date, overview, vote average, vote count, poster path, number of seasons and episodes, and TMDb ID. Use this when users ask for "best TV shows ever", "top rated series", or want quality TV recommendations. This list includes acclaimed series like Breaking Bad, Band of Brothers, Chernobyl, and other top-rated shows. Optional: page for pagination and language for localized results.

Get a list of the highest-rated TV shows of all time on TMDb
- **trending**: The mediaType parameter can be: "movie", "tv", "person", or "all" (returns mixed results with media_type field). The timeWindow parameter can be: "day" (trending today) or "week" (trending this week). Each result includes: title/name, overview, poster path, vote average, popularity score, and media type. Use this when users ask "what is trending?", "what is popular today?", or want to see what is currently hot in entertainment. The trending algorithm considers user activity, page views, and search patterns on TMDb.

Get trending content (movies, TV shows, or people) on TMDb for today or this week


## Installation & Usage

To install and use the **The Movie Database (TMDb)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-movie-database-tmdb](https://vinkius.com/mcp/the-movie-database-tmdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
