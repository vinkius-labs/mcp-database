# Stanford GDELT MCP Server

Analyze global news events and media coverage in real time with the world largest open dataset of human society.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-gdelt)

## Overview
**Category:** data-analytics
**Tools Count:** 16

## Description
Connect to the **GDELT Project API** — the world's largest open platform for monitoring global news media in real time.

### What you can do

- **Article Search** — Search global news articles with filters for language, country, date range, and topic
- **Volume Timelines** — Track how media attention to any topic changes over time
- **Sentiment Analysis** — Monitor tone and sentiment shifts in coverage of any subject
- **Geographic Mapping** — Visualize where news events are happening around the world
- **TV News Search** — Search closed caption transcripts from CNN, Fox News, MSNBC, BBC, and more
- **Theme Analysis** — Explore standardized GDELT themes across geopolitics, health, environment, and economics
- **Language Distribution** — See which linguistic communities are covering a topic
- **Country Distribution** — Identify which nations produce the most coverage of specific issues
- **Proximity Search** — Find articles where two terms appear near each other
- **Word Clouds** — Extract dominant terms and concepts from coverage

### How it works

1. Subscribe to this server
2. No API key required — GDELT is completely free
3. Start monitoring global news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists** — track breaking stories and media narratives
- **Political Scientists** — analyze geopolitical events and public discourse
- **PR & Communications** — monitor brand reputation and crisis communications
- **Policy Analysts** — understand how issues are covered across different countries and languages


## Available Tools
- **get_geo_data**: Each point includes coordinates, location name, and article metadata. Use modes: "PointData" for individual points, "PointHeat" for heatmap data.

Get geographic point data for news events
- **get_tv_channels**: Use this to understand the scope of TV news coverage available for analysis.

Get available TV news channels inventory
- **get_tv_timeline**: Reveals which stories dominate TV airtime and how TV coverage patterns differ from online news.

Get TV news mention volume timeline
- **get_themes**: GDELT uses hundreds of themes from politics, economics, health, environment, technology, and more to classify news content.

Get GDELT theme distribution for a topic
- **get_timeline_country**: Reveals geographic patterns in media attention, identifies when a story goes global, and shows which nations are most interested in specific issues.

Get source country distribution timeline
- **get_timeline_lang**: Reveals which linguistic communities are paying attention to an issue and when interest spreads across language barriers.

Get language distribution timeline for a topic
- **get_timeline_tone**: Positive values indicate positive coverage, negative values indicate negative coverage. Essential for tracking public opinion shifts, crisis communications, and brand reputation monitoring.

Get sentiment and tone timeline for a topic
- **get_timeline_volume**: Essential for tracking media attention, identifying news spikes, and understanding the lifecycle of a story. Default timespan is 3 months.

Get news volume timeline for any topic
- **get_tone_chart**: Shows whether coverage is predominantly positive, negative, or neutral, and the overall emotional intensity of the coverage.

Get tone distribution chart for a topic
- **get_word_cloud**: Reveals the dominant themes, entities, and concepts associated with a topic in media discourse.

Get word cloud data showing key terms for a topic
- **search_articles**: Returns article titles, URLs, dates, source domains, languages, and source countries. Use timespan like "1d" (1 day), "1w" (1 week), "3m" (3 months). Use sourcelang codes like "english", "spanish", "portuguese", "french", "chinese", "arabic". Use sourcecountry codes like "US", "BR", "UK", "FR", "DE".

Search global news articles across 100+ languages
- **search_by_country**: Country codes follow ISO 2-letter format: US (United States), BR (Brazil), UK (United Kingdom), FR (France), DE (Germany), CN (China), JP (Japan), IN (India), RU (Russia), AU (Australia), CA (Canada), etc. Essential for understanding country-specific media perspectives on global events.

Search news articles from a specific country
- **search_by_language**: Covers 100+ languages. Language codes include: english, spanish, portuguese, french, german, italian, chinese, japanese, korean, arabic, russian, hindi, turkish, dutch, swedish, polish, and many more. Essential for monitoring how different linguistic communities cover the same event.

Search news articles in a specific language
- **search_by_theme**: Themes are standardized topic categories like TAX_FNCACT (financial actions), HEALTH_PANDEMIC, ENV_CLIMATECHANGE, TERROR, PROTEST, ELECTION, ECON_BANKRUPTCY, etc. Use this for precise topic-based monitoring.

Search articles by GDELT standardized theme
- **search_nearby**: More precise than simple keyword search. Use distance parameter to control proximity (default 10 words). Example: term1="climate", term2="migration", distance=15.

Search articles where two terms appear near each other
- **search_tv**: Returns clips with timestamps, station names, transcript snippets, and video preview URLs. Covers CNN, Fox News, MSNBC, BBC, and more. Modes: "ClipGallery" for clips, "StationChart" for station comparison.

Search TV news transcripts by keyword


## Installation & Usage

To install and use the **Stanford GDELT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-gdelt](https://vinkius.com/mcp/stanford-gdelt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
