# Discogs MCP Server

Explore the world's largest music database — search artists, releases, labels, and marketplace listings via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/discogs)

## Overview
**Category:** ecommerce
**Tools Count:** 13

## Description
Unlock the power of the **Discogs** music database — the most comprehensive catalog of music recordings, releases, and marketplace data. Connect Discogs to your AI agent to instantly search artists, explore complete discographies, examine release details, research labels, browse marketplace listings, and analyze collector statistics — all through natural conversation.

### What you can do

- **Database Search** — Free-text search across artists, releases, labels, and tracks with filters for genre, style, year, country, and format.
- **Artist Profiles** — Retrieve complete artist information including biography, members, and full discography.
- **Release Details** — Get comprehensive metadata for any release including tracklists, formats, credits, and release history.
- **Master Releases** — Understand the canonical version of a release and explore all pressings and variants.
- **Label Research** — Explore record label catalogs, corporate structures, sublabels, and complete release histories.
- **Marketplace Intelligence** — Browse active listings, compare prices, check conditions, and find the best deals.
- **Collector Statistics** — Access community data on release popularity, wantlist counts, and sale price history.
- **User Collections** — View public collections and wantlists to understand what collectors value.

### How it works

1. Subscribe to this server
2. Enter your Discogs User Token
3. Start querying the music database through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Collectors** — research releases, compare pressings, and find fair market prices.
- **DJs and Producers** — explore discographies, research labels, and discover rare releases.
- **Music Historians** — access comprehensive metadata and release histories for academic research.
- **Record Store Owners** — price inventory, check demand, and source rare items.


## Available Tools
- **get_artist**: Returns the artist name, real name, profile/biography, members (for groups), URLs, and images. Use this after identifying an artist ID from search results.

Get detailed information about a specific artist
- **get_artist_releases**: Includes albums, singles, compilations, and credits on other releases. Results are sorted by year and include format, label, and track count. Use pagination to navigate large discographies. Returns a comprehensive overview of an artist's recorded output.

Get the complete discography of an artist
- **get_label**: Returns the label name, profile/description, parent label, sublabels, contact info, and associated releases. Use this to research label history, corporate structures, and catalog organization.

Get information about a record label
- **get_label_releases**: Returns release titles, artists, formats, catalog numbers, and release dates. Useful for researching a label's catalog, identifying rare pressings, or exploring a label's musical output. Use pagination to navigate large catalogs.

Get releases published by a specific label
- **get_marketplace_listings**: Returns seller information, price, currency, condition (media and sleeve), comments, and shipping location. Useful for finding the best deals, comparing conditions, or understanding market value. Sort by price, condition, or country. Filter by minimum/maximum condition.

Get marketplace listings for a specific release
- **get_master_release**: A master release represents the "canonical" version of a release, grouping together all individual pressings and variants. Returns the main artist, title, year, genres, styles, tracklist, and notes. Use this to understand the core creative work independent of specific pressings.

Get information about a master release
- **get_master_release_versions**: Each version represents a different pressing, reissue, or format of the same core release. Returns details including country, year, format, label, and catalog number for each version. Useful for collectors comparing different pressings or finding specific editions.

Get all versions (pressings) of a master release
- **get_release**: Returns the release title, artist, tracklist, formats, labels, catalog numbers, release date, country, genres, styles, credits, notes, and marketplace data. This is the most detailed view of a specific physical or digital release. Use this to get complete metadata for cataloging or research.

Get detailed information about a specific release
- **get_release_stats**: Returns the lowest, median, and highest sale prices, as well as the number of active listings. Useful for understanding rarity, market demand, and fair pricing for collectors.

Get community statistics and marketplace data for a release
- **get_user_collection**: Returns each release with basic metadata including artist, title, year, and format. Note: only the collection owner can see detailed information including condition, notes, and custom fields. Public collections show limited data. Use pagination to navigate large collections.

Get a user's collection of releases
- **get_user_profile**: Returns the user's location, homepage, bio, member since date, number of contributions, and collection/wantlist counts. Use this to verify user identity or get an overview of a collector's activity on the platform.

Get a Discogs user's public profile
- **get_user_wantlist**: Returns each release with basic metadata. Only the wantlist owner can see this data unless they've made it public. Useful for tracking what collectors are seeking.

Get a user's wantlist of desired releases
- **database_search**: Use the query parameter for free-text search across artists, releases, labels, and tracks. Refine results by type (artist, release, master, label, genre) and filters like genre, style, year, or country. Returns paginated results with basic metadata. Use this as the starting point for most queries. Type parameter accepts: artist, release, master, label, genre.

Search the Discogs database for artists, releases, labels, and more


## Installation & Usage

To install and use the **Discogs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discogs](https://vinkius.com/mcp/discogs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
