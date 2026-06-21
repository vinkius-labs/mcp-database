# New York Times MCP Server

Access top stories, article search, best-seller lists, and movie reviews via the NYTimes API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/new-york-times)

## Overview
**Category:** knowledge-management
**Tools Count:** 9

## Description
Connect the **New York Times** API to any AI agent and unlock access to over 170 years of journalism — including breaking news, historical archives, best-seller lists, and cultural reviews.

### What you can do
- **Top Stories** — Get the latest top stories for any section (World, Politics, Tech, Sports, etc.)
- **Article Search** — Search the complete archive from 1851 to the present day with keywords and date filters
- **Most Popular** — See what readers are emailing, sharing, and viewing the most
- **Best-Seller Lists** — Retrieve current and historical book best-seller lists
- **Movie Reviews** — Access thousands of movie reviews and critic summaries
- **Section Discovery** — List all available sections and topics covered by the NYTimes

### How it works
1. Subscribe to this server
2. Enter your NYTimes Developer API Key
3. Start exploring world-class journalism from Claude, Cursor, or any MCP-compatible client

The NYTimes API is free for development use, providing a generous limit of requests per day.

### Who is this for?
- **Researchers & Historians** — Track how events were reported over decades using the extensive archive
- **Journalists & Writers** — Find background context and related coverage for current events
- **Book Lovers** — Check weekly best-seller lists and discover trending authors
- **Cinephiles** — Explore the Paper of Record's vast collection of film criticism


## Available Tools
- **get_archive**: Get all articles for a specific month
- **get_book_lists**: "list_name_encoded" is the list slug (e.g., "hardcover-fiction"). Optional date is YYYY-MM-DD.

Get current or historical best-seller lists
- **get_most_emailed**: Period can be 1, 7, or 30 days.

Get the most emailed articles for a specific period
- **get_most_shared**: Period can be 1, 7, or 30 days.

Get the most shared articles on social media
- **get_most_viewed**: Get the most viewed articles
- **get_movie_reviews**: Optional "query" filters by movie title.

Search for movie reviews in the NYTimes archive
- **search_articles**: Use "q" for keywords, "begin_date" and "end_date" for date ranges (YYYYMMDD), and "sort" for "newest", "oldest", or "relevance".

Search for articles using keywords, date ranges, and sorting
- **get_sections**: List all available news sections
- **get_top_stories**: g., home, world, politics, technology, sports). Use get_sections to see available options.

Get top stories for a specific section


## Installation & Usage

To install and use the **New York Times** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/new-york-times](https://vinkius.com/mcp/new-york-times)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
