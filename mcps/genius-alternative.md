# Genius MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genius-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest collection of song lyrics and musical knowledge. Search songs, artists, and annotations directly from your AI agent.

## Description
Connect your **Genius** account to any AI agent to explore the world's largest database of song lyrics and crowdsourced musical knowledge.

### What you can do

- **Search & Discovery** — Use `search` to find songs and artists or `lookup_web_page` to find Genius data for any URL.
- **Lyrics & Annotations** — Retrieve deep insights into song meanings with `get_annotation` and `get_referents`.
- **Artist Insights** — Fetch comprehensive artist profiles and their discography using `get_artist` and `get_artist_songs`.
- **Community Interaction** — Upvote, downvote, or create your own annotations using `upvote_annotation`, `downvote_annotation`, and `create_annotation`.
- **Account Management** — Access your own profile details with `get_account`.

### How it works

1. Subscribe to this server
2. Enter your Genius Client Access Token
3. Start exploring musical context from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — dive deep into the hidden meanings of your favorite tracks without leaving your chat interface.
- **Content Creators** — quickly verify lyrics and artist facts for videos, blogs, or social media.
- **Developers** — integrate musical metadata and annotations into your workflow seamlessly.


## Available Tools (14)
- **create_annotation**: Requires create_annotation scope.

Create a new annotation on a public web page
- **delete_annotation**: Requires manage_annotation scope.

Delete an annotation
- **downvote_annotation**: Requires vote scope.

Downvote an annotation
- **get_account**: Requires me scope.

Get current user account information
- **get_annotation**: Get data for a specific annotation
- **get_artist_songs**: Get songs by a specific artist
- **get_artist**: Get data for a specific artist
- **get_referents**: Get referents (sections of content with annotations)
- **get_song**: Get data for a specific song
- **lookup_web_page**: Lookup a web page on Genius
- **search**: Search all song content hosted on Genius
- **unvote_annotation**: Requires vote scope.

Remove vote from an annotation
- **update_annotation**: Requires manage_annotation scope.

Update an annotation
- **upvote_annotation**: Requires vote scope.

Upvote an annotation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genius** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the song 'Bohemian Rhapsody' and give me its ID."

**🤖 AI Agent:**
> I found 'Bohemian Rhapsody' by Queen. The Song ID is 63214. Would you like me to fetch the full details or annotations for this track?

---

**👤 You:**
> "Get all songs by the artist with ID 16775."

**🤖 AI Agent:**
> Fetching songs for Artist ID 16775 (Kendrick Lamar)... I've found tracks like 'HUMBLE.', 'DNA.', and 'Alright'. Would you like to see the full list or details for a specific song?

---

**👤 You:**
> "What does the annotation with ID 1034 say?"

**🤖 AI Agent:**
> Annotation 1034 explains the historical context of the opening verse, noting that the artist is referencing a specific event from 1969. It has 45 upvotes.


## ❓ FAQ

**Q: Can I search for a song if I only know a few words of the lyrics?**
Yes! Use the `search` tool with the lyrics you remember. The agent will return the most relevant song matches from the Genius database.

**Q: How do I see the meaning behind a specific line in a song?**
You can use `get_referents` with a `song_id` to see all annotated sections, or `get_annotation` with a specific ID to read the detailed community explanation.

**Q: Is it possible to vote on annotations through the AI?**
Absolutely. You can use `upvote_annotation`, `downvote_annotation`, or `unvote_annotation` by providing the Annotation ID, provided your token has the necessary scopes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genius-alternative](https://vinkius.com/mcp/genius-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Genius** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `genius-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Genius** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "genius-alternative": {
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
