# Chess.com MCP Server

Access Chess.com player profiles, stats, games, puzzles, and leaderboards directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/chesscom)

## Overview
**Category:** education
**Tools Count:** 15

## Description
Connect to the **Chess.com** public API and explore the entire chess ecosystem through natural conversation. No authentication required — just install and start querying immediately.

### What you can do

- **Player Profiles & Stats** — Fetch any player display name, avatar, join date, follower count, plus detailed ratings across all time controls (bullet, blitz, rapid, daily) and puzzle rush scores
- **Online Status** — Check if a player is currently connected to Chess.com in real-time
- **Game History** — Retrieve all finished games for any month with full PGN data, opponent info, opening names, accuracy ratings, and game results
- **Daily & Current Games** — See which correspondence games a player currently has in progress
- **Puzzles** — Get the official daily puzzle or fetch unlimited random puzzles for tactical training
- **Clubs** — Explore Chess.com clubs, view member rosters, and discover community affiliations
- **Leaderboards** — See the highest-rated players across all game types on Chess.com
- **Titled Players** — Lists of GMs, IMs, FMs, WGMs, NMs, and other officially titled players
- **Streamers** — Find verified Chess.com content creators across Twitch, YouTube, and other platforms
- **Country Players** — Discover players from any nation using ISO country codes

### How it works

1. Subscribe to this server
2. No API key or authentication needed — the Chess.com API is fully public
3. Start exploring chess data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Chess Players** — analyze your own game history, check opponent stats, and find training puzzles without leaving your AI chat
- **Coaches & Content Creators** — quickly pull player statistics, game records, and leaderboard data for analysis or streaming prep
- **Chess Enthusiasts** — explore titled player lists, discover streamers to watch, and track the strongest players worldwide


## Available Tools
- **get_club_info**: com club by its URL identifier. Returns the club name, description, creation date, last activity date, visibility status, admin information, and total member count. Use this tool to learn about a club before joining, verify club existence, or gather metadata about chess communities.

Get information about a Chess.com club
- **get_club_members**: com club. Each entry includes the member username and their profile URL. Use this tool to discover active players within a specific club community, find potential opponents who share your chess interests, or identify titled players within a club roster.

Get weekly active members of a Chess.com club
- **get_country_players**: com players who have registered with a specific country. Takes an ISO 3166-1 country code (e.g., "US" for United States, "BR" for Brazil, "IN" for India, "RU" for Russia, "NO" for Norway). Returns an array of player usernames affiliated with that country. Use this tool to discover players from a specific nation, find local opponents, or research the chess scene in different countries.

Get Chess.com players from a specific country
- **get_daily_puzzle**: com daily puzzle including the puzzle position (FEN), the sequence of moves for the solution, the puzzle rating, and the associated game metadata (players, result, opening). Use this tool to get a tactical puzzle to solve, practice chess tactics, or study interesting positions from real games. The puzzle changes once per day.

Get the Chess.com daily puzzle
- **get_leaderboards**: com leaderboards showing the highest-rated players across different game categories. Returns top players for daily chess (correspondence), blitz, bullet, and rapid time controls, plus puzzle rush leaders. Each entry includes username, current rating, and profile URL. Use this tool to identify the strongest active players on Chess.com, track rating leaders, or find grandmaster accounts to study.

Get Chess.com leaderboards for top players
- **get_player_clubs**: com clubs that a specific player belongs to. Returns club names, URLs, creation dates, and membership counts. Use this tool to discover a player community affiliations, find clubs with similar interests, or identify potential clubs to join based on where strong players are members.

Get clubs that a Chess.com player is a member of
- **get_player_current_games**: com player. Returns game details including opponent username, current position (FEN), time control, last activity date, and game URL. Use this tool to check what ongoing games a player has, see who they are playing against in daily chess, or monitor active correspondence matches. Does not include live (real-time) games that are currently being played.

Get a player's currently active daily (correspondence) games
- **get_player_game_archives**: com player. Each URL corresponds to a specific year/month combination where the player has recorded games. Use this tool to discover which months have available game data before fetching actual games with get_player_monthly_games. The returned URLs can be parsed to extract year and month parameters.

Get list of available game archive URLs for a player
- **get_player_monthly_games**: com player during a specific year and month. Returns detailed PGN data, game results, opponent usernames, opening names, time controls, accuracy ratings (if available), and game end reasons. Use this tool to analyze a player game history, study their openings, review losses against specific opponents, or collect training data. Month is 1-indexed (January = 1, December = 12).

Get all finished games for a player in a specific month
- **get_player_profile**: com player by username. Returns the player display name, avatar URL, join date, last online timestamp, follower count, country, and title if applicable (GM, IM, FM, etc.). Use this tool to verify a username exists and gather basic identity information about a Chess.com player before querying their stats or games.

Get Chess.com player profile information
- **get_player_stats**: com player. Returns current and best ratings across all game types (chess_rapid, chess_blitz, chess_bullet, chess_daily, puzzle_rush, lessons), plus win/loss/draw records for each time control. Use this tool to evaluate a player skill level, check their peak ratings, or compare performance across different time controls.

Get Chess.com player statistics including ratings and records
- **get_random_puzzle**: com puzzle database. Returns the puzzle position (FEN), the complete solution moves, puzzle rating, and the source game information (white player, black player, result, opening name). Use this tool for unlimited tactical practice sessions, training sessions, or when you want a fresh puzzle that is not the daily puzzle.

Get a random chess puzzle from Chess.com
- **get_streamers**: com verified streamers. Each entry includes the streamer username, streaming platform (Twitch, YouTube, etc.), stream URL, language, and follower count. Use this tool to find chess content creators to watch, discover educational streams in your preferred language, or locate titled players who regularly broadcast their games.

Get the list of official Chess.com streamers
- **get_titled_players**: com players who hold a specific chess title. Supported titles include: GM (Grandmaster), IM (International Master), FM (FIDE Master), CM (Candidate Master), WGM (Woman Grandmaster), WIM (Woman International Master), WFM (Woman FIDE Master), WCM (Woman Candidate Master), NM (National Master), and LM (Legends Master). Returns an array of usernames. Use this tool to find all grandmasters on Chess.com, locate titled players for study, or verify if a player holds an official title.

Get list of titled players by title type
- **is_player_online**: com player. Returns a simple status object indicating whether the player is currently connected to Chess.com servers. Useful for determining if a daily chess opponent or streamer is actively playing right now before attempting to challenge them.

Check if a Chess.com player is currently online


## Installation & Usage

To install and use the **Chess.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chesscom](https://vinkius.com/mcp/chesscom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
