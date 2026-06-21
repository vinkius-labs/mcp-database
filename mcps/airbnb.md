# Airbnb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airbnb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search and manage Airbnb listings, experiences, reservations, and pricing directly from any AI agent.

## Description
Connect your **Airbnb** account to any AI agent and take full control of travel planning, accommodation search, and reservation management through natural conversation.

### What you can do

- **Search Listings** — Find Airbnb properties by city, neighborhood, or address with filters for dates, guests, and price range
- **Listing Details** — Get complete property information including amenities, photos, house rules, and cancellation policies
- **Guest Reviews** — Read reviews from previous guests to assess quality, accuracy, and host responsiveness
- **Availability Calendar** — Check which dates are available or booked for any listing before planning your trip
- **Pricing Breakdown** — See detailed pricing including nightly rate, cleaning fee, service fee, and total cost
- **Experiences** — Discover local activities, tours, and events hosted by locals in your destination
- **Reservation Management** — View upcoming trips, completed stays, and cancelled reservations
- **Host Information** — Check host profile, response rate, and other properties they manage

### How it works

1. Subscribe to this server
2. Enter your Airbnb API key
3. Start searching accommodations, checking availability, and managing reservations from Claude, Cursor, or any MCP-compatible client

No more browsing hundreds of listings manually. Your AI acts as a dedicated travel agent.

### Who is this for?

- **Travelers** — instantly find available accommodations matching dates, budget, and preferences without scrolling through endless listings
- **Trip Planners** — compare pricing breakdowns, read reviews, and check availability calendars before booking
- **Business Travel** — quickly find suitable accommodations near meeting locations using coordinate-based search
- **Experience Seekers** — discover unique local activities and tours alongside accommodation search


## Available Tools (12)
- **get_calendar**: This helps plan trips by confirming availability before attempting to book.
You can optionally specify a month (YYYY-MM format) to view a specific month's calendar.
The response shows available dates, minimum stay requirements, and pricing variations by date.

Check availability calendar for an Airbnb listing
- **get_experience**: Use the experience_id from search_experiences to inspect full activity details before booking.
This helps travelers understand what the experience entails and whether it matches their interests.

Get detailed information about an Airbnb Experience
- **get_host**: This helps guests evaluate host reliability and trustworthiness before booking.
Use the host_id obtained from listing details to inspect host credentials.

Get details about a listing host
- **get_listing**: Use the listing_id obtained from search_listings to inspect full property details before booking.
This includes bed/bath counts, capacity, check-in instructions, and guest reviews summary.

Get detailed information about a specific Airbnb listing
- **get_pricing**: You must provide check-in and check-out dates.
Optionally specify number of guests as pricing may vary based on occupancy.
This helps travelers understand the full cost before booking, including all fees and taxes.

Get detailed pricing for an Airbnb listing
- **get_reservation**: Use the reservation_id obtained from get_reservations to inspect specific booking details.
This is useful for reviewing trip details, confirming booking status, or preparing for check-in.

Get detailed information about a specific reservation
- **get_reservations**: Shows upcoming trips, completed stays, and cancelled reservations.
Optionally filter by status (upcoming, completed, cancelled) and limit the number of results.
Each reservation includes listing details, dates, total price, and host information.
Use this to review travel history or check upcoming trip details.

Get current and past reservations for the authenticated user
- **get_reviews**: Use the listing_id from search_listings to see what previous guests have said about their stay.
Reviews help assess the quality, accuracy of listing description, host responsiveness, and overall guest experience.
Optionally limit the number of reviews returned (default: all available).

Get reviews for a specific Airbnb listing
- **get_user_profile**: Use this to verify account access and view your profile details.

Get the authenticated user profile
- **search_by_coordinates**: This is useful for finding accommodations near a specific point of interest or when you know exact coordinates.
Optionally specify a search radius in kilometers, check-in/check-out dates, and number of guests.
Results are sorted by proximity to the specified coordinates.

Search listings by geographic coordinates
- **search_experiences**: Experiences are unique activities hosted by locals, from food tours to adventure activities.
Optionally specify a date to see what's available on a specific day.
Results include experience name, host, duration, price, rating, and booking links.
This helps travelers discover local activities beyond just accommodation.

Search Airbnb Experiences in a location
- **search_listings**: You can search by city name, neighborhood, or address. Optionally specify check-in and check-out dates (YYYY-MM-DD format),
number of guests, and minimum/maximum price per night. This helps find available accommodations matching traveler preferences.
Results include listing name, location, price, rating, amenities, and booking links.

Search Airbnb listings by location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airbnb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Airbnb listings in Paris for 2 guests, checking in March 15th and checking out March 20th, 2026."

**🤖 AI Agent:**
> I found 15 available listings in Paris for March 15-20, 2026. Top options: 1. **Charming Marais Apartment** — €120/night, ⭐4.92 (324 reviews), sleeps 4, entire home
2. **Eiffel Tower View Studio** — €185/night, ⭐4.95 (512 reviews), sleeps 2, Superhost
3. **Montmartre Artist Loft** — €95/night, ⭐4.87 (198 reviews), sleeps 3, entire home

Would you like detailed information, pricing breakdown, or availability calendar for any of these?

---

**👤 You:**
> "What Airbnb experiences are available in Tokyo on April 5th, 2026?"

**🤖 AI Agent:**
> I found 8 experiences in Tokyo for April 5th, 2026:
1. **Traditional Tea Ceremony in Asakusa** — ¥4,500/person, ⭐4.96 (287 reviews), 2 hours
2. **Shibuya Night Food Tour** — ¥8,900/person, ⭐4.93 (456 reviews), 3.5 hours
3. **Tsukiji Market & Sushi Making Class** — ¥12,000/person, ⭐4.98 (612 reviews), 4 hours
4. **Akihabara Anime & Manga Walking Tour** — ¥3,800/person, ⭐4.85 (198 reviews), 2.5 hours

Would you like full details about any of these experiences?

---

**👤 You:**
> "Show me my upcoming reservations and check the availability calendar for my next trip."

**🤖 AI Agent:**
> You have 2 upcoming reservations:
1. **Lisbon Riverside Apartment** — March 22-27, 2026 (5 nights) — €450 total — Host: Maria (98% response rate)
2. **Barcelona Gothic Quarter Flat** — April 10-14, 2026 (4 nights) — €380 total — Host: Carlos (Superhost)

I've checked the availability calendar for your Lisbon trip: the dates March 22-27 are confirmed and reserved. Would you like the check-in instructions or details about the neighborhood?


## ❓ FAQ

**Q: How do I get an Airbnb API key?**
Airbnb's API access is available through their partner program. Visit the Airbnb partner portal, apply for API access, and upon approval you'll receive your API credentials. Alternatively, many travel data aggregators provide Airbnb data via API keys that can be used with this server.

**Q: Can I search for listings in multiple cities at once?**
Yes! Simply run the `search_listings` tool multiple times with different location parameters. The AI agent can compare results across cities, helping you choose the best destination based on price, availability, and ratings.

**Q: Can I book a listing directly through this integration?**
This integration focuses on search, discovery, and information retrieval. You can find available listings, check pricing, read reviews, and verify availability. To complete a booking, you'll need to use the Airbnb website or app directly. The AI agent can provide booking links for each listing found.

**Q: What are Airbnb Experiences and how can I find them?**
Airbnb Experiences are unique activities hosted by locals — from food tours and cooking classes to adventure sports and cultural workshops. Use the `search_experiences` tool with a location to discover activities in your destination. You can also filter by date to see what's available during your stay. Each experience includes details about what's included, meeting point, duration, and reviews from previous participants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airbnb](https://vinkius.com/mcp/airbnb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airbnb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airbnb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airbnb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airbnb": {
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
