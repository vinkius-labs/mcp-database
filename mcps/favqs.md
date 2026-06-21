# Favqs MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/favqs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/favqs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/favqs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Discover and manage quotes — fetch the Quote of the Day, search by author or tag, and curate your favorites directly via AI.

## Description
Connect **Favqs** to your AI agent to access a world of inspiration and wisdom. Whether you are looking for the perfect quote for a presentation or building a personal library of sayings, this MCP server provides full access to the Favqs database.

### What you can do

- **Daily Inspiration** — Use `get_qotd` to start your day with the featured Quote of the Day.
- **Advanced Search** — Use `list_quotes` to find specific wisdom by filtering for authors, tags, or keywords.
- **Personal Library** — Favorite (`favorite_quote`), tag (`tag_quote`), or upvote quotes to save them to your account.
- **Community Features** — Follow other users (`follow`) and track their activity to discover new content.
- **Content Creation** — Add your own quotes (`add_quote`) or update existing ones to share with the community.

### How it works

1. Subscribe to this server
2. Enter your Favqs App Token
3. (Optional) Use `create_session` to get a User Token for personalized actions
4. Start exploring quotes from Claude, Cursor, or any MCP client

### Who is this for?

- **Writers & Bloggers** — Quickly find and verify quotes to enrich your content.
- **Social Media Managers** — Automate the discovery of engaging daily content.
- **Personal Development Enthusiasts** — Maintain a curated list of quotes that resonate with your goals.


## Available Tools
- **add_quote**: Add a new quote (User Session Required)
- **clearvote_quote**: Clear vote on a quote (User Session Required)
- **create_session**: Create a user session to obtain a User-Token
- **create_user**: Create a new FavQs user
- **delete_quote**: Delete a private quote (Pro only)
- **destroy_session**: Destroy the current user session
- **downvote_quote**: Downvote a quote (User Session Required)
- **favorite_quote**: Favorite a quote (User Session Required)
- **follow**: Follow a user, author, or tag
- **forgot_password**: Request a password recovery email
- **get_activity**: Get activity feed
- **get_followers**: Get followers of the current user
- **get_following**: Get entities the current user is following
- **get_qotd**: Does not require authentication.

Get the Quote of the Day
- **get_quote**: Get a specific quote by ID
- **get_typeahead**: Get a list of public Authors, Tags, and Users for autocomplete
- **get_user**: Get a user profile
- **hide_quote**: Hide a quote (User Session Required)
- **list_quotes**: List and search quotes
- **publicize_quote**: Make a private quote public (Pro only)
- **reset_password**: Reset password using a recovery token
- **tag_quote**: Add personal tags to a quote (User Session Required)
- **unfavorite_quote**: Unfavorite a quote (User Session Required)
- **unfollow**: Unfollow a user, author, or tag
- **unhide_quote**: Unhide a quote (User Session Required)
- **update_quote**: Update a private quote (Pro only)
- **update_user**: Update a user profile
- **upvote_quote**: Upvote a quote (User Session Required)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Favqs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the quote of the day."

**🤖 AI Agent:**
> The Quote of the Day is: 'Life is what happens when you're busy making other plans.' - John Lennon. Would you like to save this to your favorites?

---

**👤 You:**
> "Find some quotes about 'courage' by Winston Churchill."

**🤖 AI Agent:**
> I found several quotes. One notable one is: 'Success is not final, failure is not fatal: it is the courage to continue that counts.' Should I list more from this author?

---

**👤 You:**
> "Favorite the quote with ID 12345."

**🤖 AI Agent:**
> I've successfully added quote 12345 to your favorites. You can view your full list of favorites anytime using `list_quotes`.


## Installation & Usage

To install and use the **Favqs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/favqs](https://vinkius.com/mcp/favqs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
