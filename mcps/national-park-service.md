# National Park Service MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/national-park-service)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/national-park-service-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/national-park-service-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access authoritative data about U.S. National Parks via NPS — track alerts, parks, and events directly from your AI agent.

## Description
Connect to the **National Park Service (NPS)** API through your AI agent and explore authoritative information about U.S. National Parks using natural conversation.

### What you can do

- **Park Discovery** — List parks by state or specific park code to get descriptions, hours, and location info.
- **Real-time Alerts** — Stay informed with up-to-date safety alerts, closures, and important notices for any park.
- **Camping & Facilities** — Access detailed data on campgrounds and available facilities across the park system.
- **Event Tracking** — Find upcoming scheduled activities and events happening in the parks.
- **Educational Resources** — Retrieve articles, lesson plans, and news releases for academic or personal interest.
- **Live Webcams** — Get metadata and links for live streaming cameras to see park conditions in real-time.
- **Visitor Centers & Places** — Locate visitor centers and significant points of interest within the parks.

### How it works

1. Subscribe to this server
2. Enter your NPS API Key (get one for free at nps.gov/subjects/developer)
3. Start exploring U.S. National Parks from Claude, Cursor, or any MCP client

### Who is this for?

- **Travelers & Hikers** — quickly check for alerts or campground availability while planning your next trip.
- **Nature Enthusiasts** — discover events and view live webcams from your favorite parks.
- **Educators & Students** — retrieve authoritative metadata and lesson plans for research or curriculum development.


## Available Tools
- **list_alerts**: List park alerts and closures
- **list_articles**: List park articles
- **list_campgrounds**: List park campgrounds
- **list_events**: List scheduled park events
- **list_lesson_plans**: List park lesson plans
- **list_news_releases**: List official news releases
- **list_parks**: Can filter by park code or state.

List U.S. National Parks
- **list_places**: List significant park places
- **list_visitor_centers**: List park visitor centers
- **list_webcams**: List park streaming webcams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **National Park Service** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all national parks in California."

**🤖 AI Agent:**
> I've retrieved the parks for California. You have several notable ones including 'Yosemite National Park' (YOSE), 'Joshua Tree National Park' (JOTR), and 'Death Valley National Park' (DEVA). Shall I check for active alerts in Yosemite?

---

**👤 You:**
> "Are there any active safety alerts for Yellowstone?"

**🤖 AI Agent:**
> I've checked the alerts for Yellowstone (YELL). There are 2 active notices: a 'Caution' due to high bear activity in certain areas and a 'Notice' about a seasonal road closure on Dunraven Pass. Would you like more details on the bear activity areas?

---

**👤 You:**
> "Show me upcoming events in Grand Canyon."

**🤖 AI Agent:**
> Retrieving events for Grand Canyon (GRCA)... There is a 'Guided Rim Walk' scheduled for tomorrow at 10 AM and a 'Star Party' this Saturday evening. Shall I provide the meeting location for the rim walk?


## Installation & Usage

To install and use the **National Park Service** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/national-park-service](https://vinkius.com/mcp/national-park-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
