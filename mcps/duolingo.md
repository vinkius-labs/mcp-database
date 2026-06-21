# Duolingo MCP Server

Track language learning progress on Duolingo — view profiles, streaks, XP, leaderboards and dictionary hints.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/duolingo)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect to **Duolingo** and explore language learning progress through natural conversation — no API key needed for public data.

### What you can do

- **User Profiles** — View any user's public profile including XP, streak, language and skill progress
- **Version Info** — Get API version info including supported languages and features
- **Dictionary Hints** — Get translation hints between any two supported languages
- **Store Items** — Browse Duolingo store items like streak freezes and power-ups
- **Leaderboards** — View leaderboard rankings by XP for users and languages
- **Friends** — See a user's friends list with their streaks and XP

### How it works

1. Subscribe to this server
2. No API key needed for public endpoints
3. Start exploring Duolingo data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Language Learners** — track your XP, streak and compare with friends on leaderboards
- **Teachers** — monitor student progress and engagement on Duolingo
- **App Developers** — build language learning tools using Duolingo's public data


## Available Tools
- **get_daily_leaderboard**: Shows top users by XP for the current day. Optionally specify language code and timezone.

Get daily leaderboard for a language
- **get_dictionary_hints**: Returns translation pairs for the given tokens. Useful for building flashcards or vocabulary tools. Target and source are language codes (e.g. "es", "fr", "de", "en").

Get dictionary hints for word translations
- **get_friends**: Optionally provide a user ID. Returns friend usernames, IDs, streaks and XP totals.

Get Duolingo friends list
- **get_leaderboard**: Optionally provide a user ID to get leaderboard info for a specific user. Returns rankings with usernames, XP totals and positions.

Get Duolingo leaderboard data
- **get_store_items**: Requires authentication for full details. Returns item IDs, names, prices and descriptions.

Get Duolingo store items
- **get_user_by_id**: Returns the same data as get_user_by_username but uses the numeric ID instead.

Get a Duolingo user profile by user ID
- **get_user_by_username**: Returns username, user ID, avatar, current language, total XP, streak, skills and progress. Note: Full profile data (detailed progress, skill trees) requires authentication and only works for your own account.

Get a Duolingo user profile by username
- **get_version_info**: Useful for understanding available language codes and API capabilities.

Get Duolingo API version information


## Installation & Usage

To install and use the **Duolingo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duolingo](https://vinkius.com/mcp/duolingo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
