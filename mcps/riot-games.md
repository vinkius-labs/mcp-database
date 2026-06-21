# Riot Games MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/riot-games)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/riot-games-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/riot-games-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access League of Legends player data — summoner profiles, match history, ranked stats, champion masteries and live games.

## Description
Connect to **Riot Games API** and access League of Legends player data through natural conversation.

### What you can do

- **Player Lookup** — Find any player by Riot ID (game name + tag line) and get their PUUID
- **Summoner Profile** — Get summoner level, profile icon and account details
- **Match History** — Browse recent matches with full details (KDA, items, runes, gold, damage)
- **Ranked Stats** — Check current rank, tier, LP and win/loss records for all queues
- **Champion Masteries** — View champion mastery levels, points and tokens
- **Live Games** — Check if a player is currently in-game with team compositions and bans
- **Featured Games** — Browse high-elo live games currently in progress
- **Champion Data** — Get full champion info including abilities, stats, lore and skins

### How it works

1. Subscribe to this server
2. Enter your Riot Games API Key (free registration at developer.riotgames.com)
3. Start exploring League of Legends data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Players** — check your ranked stats, match history, champion masteries and live games
- **Coaches & Analysts** — analyze player performance, match data and ranked distributions
- **Content Creators** — access player data, live games and champion info for content


## Available Tools
- **get_account_by_puuid**: Returns game name, tag line and account metadata.

Get player account details by PUUID
- **get_account_by_riot_id**: Returns the PUUID (Player Universally Unique Identifier), game name, tag line and account metadata. The PUUID is required for most other API calls.

Get player account by Riot ID (game name + tag line)
- **get_active_game**: Returns game mode, game type, banned champions, all players with their champions, summoner spells, runes and team info. Returns 404 if the summoner is not in a game. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get current live game for a summoner
- **get_champion_details**: Uses Data Dragon (static data, no API key needed).

Get detailed info for a specific champion
- **get_champion_masteries**: Returns champion ID, mastery level (1-7), mastery points, last play time, chest earned status and tokens needed for next level. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get champion mastery data for a player
- **get_champions**: Uses Data Dragon (static data, no API key needed). Optional version (e.g. "14.1.1") and locale (e.g. "en_US", "pt_BR").

Get all League of Legends champions
- **get_featured_games**: Returns game mode, banned champions, all players with their champions, summoner spells and game length. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get currently featured games (high elo live games)
- **get_league_entries**: Returns tier (IRON, BRONZE, SILVER, GOLD, PLATINUM, EMERALD, DIAMOND, MASTER, GRANDMASTER, CHALLENGER), rank (I-IV), LP, wins, losses and hot/streak info. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get ranked league entries for a summoner
- **get_match**: Requires the regional routing where the match was played (americas, europe, asia, sea).

Get detailed match data by match ID
- **get_match_ids**: Returns up to 20 match IDs by default. Use count (1-100) to get more matches and start for pagination. Regional routing: americas (NA, BR, LAN, LAS), europe (EUW, EUNE, TR, RU), asia (KR, JP), sea (PH, SG, TH, TW, VN, OCE).

Get match history (match IDs) for a player
- **get_summoner_by_id**: Returns summoner level, profile icon ID, revision date and account ID. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get League of Legends summoner profile by summoner ID
- **get_summoner_by_puuid**: The summoner ID is needed for league and spectator queries. Platform codes: br1, na1, euw1, eun1, kr, jp1, oc1, la1, la2, tr1, ru.

Get League of Legends summoner profile by PUUID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Riot Games** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the summoner Faker on KR server."

**🤖 AI Agent:**
> Faker#KR1 found. Summoner Level: 687. PUUID: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. Summoner ID: xxxxxxxxxxxxxx.

---

**👤 You:**
> "What's Faker's ranked stats on KR?"

**🤖 AI Agent:**
> Solo/Duo: Challenger I, 1456 LP, 412W/298L (58.0% WR). Flex: Master I, 234 LP, 89W/67L (57.1% WR). Hot streak: true.

---

**👤 You:**
> "Get Faker's last 5 match IDs."

**🤖 AI Agent:**
> Found 5 recent matches: KR_7234567890, KR_7234567889, KR_7234567888, KR_7234567887, KR_7234567886. Use get_match to see full details for any match.


## Installation & Usage

To install and use the **Riot Games** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/riot-games](https://vinkius.com/mcp/riot-games)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
