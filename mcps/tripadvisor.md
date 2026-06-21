# TripAdvisor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tripadvisor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tripadvisor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tripadvisor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search hotels, restaurants, and attractions via TripAdvisor Content API — get reviews, ratings, and POI details.

## Description
Connect your AI agent to the world's largest travel platform. The TripAdvisor Content API integration allows you to discover and inspect destinations, accommodations, and dining experiences with real-time data from millions of users.

### What you can do

- **POI Discovery** — Find any location by name, address, or geographic coordinates
- **Trusted Reviews** — Read the latest user feedback and detailed ratings to make informed travel decisions
- **Visual Content** — Fetch high-quality professional and traveler photos of hotels and attractions
- **Deep Insights** — Access specific metadata like price levels, rankings, and award information
- **Nearby Exploration** — Search for the best restaurants or hotels around a specific GPS coordinate

### How it works

1. Subscribe to this server
2. Enter your **TripAdvisor API Key** (obtained via the TripAdvisor Developer Portal)
3. Start planning and researching travel destinations directly through chat

### Who is this for?

- **Travel Enthusiasts** — research and plan your next trip without leaving your chat
- **Concierge Services** — quickly find and vet recommendations for clients
- **Data Analysts** — explore travel trends and location-based sentiment


## Available Tools
- **get_location_details**: Get comprehensive details for a specific location using its ID
- **get_location_photos**: Retrieve professional and user photos for a specific location
- **get_location_reviews**: Retrieve the latest user reviews for a specific location
- **get_nearby_locations**: Search for locations near a specific geographic coordinate
- **search_location**: Search for hotels, restaurants, and attractions by name or address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TripAdvisor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for top-rated attractions in Paris."

**🤖 AI Agent:**
> I've found several top attractions in Paris, including the Eiffel Tower (Location ID: 188757) and the Louvre Museum (Location ID: 188757). Would you like to see reviews for any of them?

---

**👤 You:**
> "Show me photos and details for location ID 188151."

**🤖 AI Agent:**
> Retrieving data for Location ID 188151... It's the Colosseum in Rome. It has a 4.5 rating with over 150k reviews. Here are some photos of the landmark.


## Installation & Usage

To install and use the **TripAdvisor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tripadvisor](https://vinkius.com/mcp/tripadvisor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
