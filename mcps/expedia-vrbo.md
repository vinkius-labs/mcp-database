# Expedia Vrbo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia-vrbo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate vacation rental research via Vrbo — search entire homes, compare nightly rates, and check availability calendars directly from any AI agent.

## Description
Connect your **Expedia Rapid API** account to any AI agent and access Vrbo's global inventory of vacation rental properties — entire homes, condos, and unique stays.

### What you can do

- **Rental Search** — Find vacation homes by destination, dates, guest count, and property type with real-time availability
- **Property Details** — Retrieve full property descriptions, amenity lists, house rules, and exact map coordinates for any listing
- **Availability Calendars** — Check open dates and nightly rates across weeks or months to find the best booking window
- **Photo Galleries** — Access high-resolution property images for visual comparison before booking
- **Booking & Cancellation** — Reserve properties and manage existing itineraries programmatically through the API

### How it works

1. Sign up at the [Expedia Group Developer Hub](https://developers.expediagroup.com/) and create a Rapid API project
2. Generate your API Key and Shared Secret from the portal
3. Enter your credentials here and start searching vacation rentals from Claude, Cursor, or any MCP-compatible client

Your agent becomes a vacation rental concierge — scanning hundreds of entire-home listings to find the perfect stay without browsing dozens of pages.

### Who is this for?

- **Vacation Planners** — find and compare entire homes across destinations, matching group size, amenities, and budget in one conversation
- **Property Managers** — monitor competitor listings, pricing trends, and availability patterns across markets
- **Event Organizers** — locate multi-bedroom properties near event venues that accommodate large groups


## Available Tools (11)
- **book_rental**: Requires the rental property ID, check-in and check-out dates, guest details (primary guest name, email, phone), and payment information. This is a write action that will create an actual itinerary. Ensure all details are confirmed before executing.

Book a vacation rental property
- **cancel_itinerary**: This is a destructive write action. The cancellation policy of the rental property will determine whether a full, partial, or no refund is applicable. Always confirm the itinerary ID and cancellation reason before executing. The guest will receive a confirmation email upon successful cancellation.

Cancel an existing vacation rental booking
- **check_rental_policies**: Use this to inform the user about restrictions and obligations before booking.

Get the policies and rules for a vacation rental property
- **get_itinerary**: Use this to look up a confirmed reservation by its itinerary ID.

Get details of an existing vacation rental booking itinerary
- **get_rental_calendar**: Use this to check date flexibility or understand pricing variations across different dates.

Get the availability calendar for a vacation rental
- **get_rental_details**: Use this after search_rentals to evaluate a specific property before booking.

Get full details for a specific vacation rental property
- **get_rental_images**: Each image includes URLs, captions, category tags, and dimensions. Use this when the user wants to visually inspect a property before making a booking decision.

Get all photos and images for a vacation rental property
- **get_rental_reviews**: Returns individual review entries with overall ratings, category scores (cleanliness, communication, location, value), review text, traveler name, travel dates, and submission dates. Use this to help the user evaluate a rental property based on real guest experiences. Especially useful for comparing properties or verifying quality before booking.

Get guest reviews and ratings for a vacation rental property
- **get_unit_amenities**: Returns structured amenity data including categories (kitchen, bathroom, entertainment, outdoor, safety), individual amenity names, descriptions, and availability status. Use this when the user needs to verify specific amenities like pool, wifi, parking, pet-friendliness, or accessibility features.

Get the full list of unit amenities for a vacation rental
- **search_rental_regions**: Returns region IDs, names, types (city, neighborhood, airport, poi), and coordinates. Use this as a first step when the user provides a destination name instead of a destination_id, to resolve the name into a valid region ID for search_rentals.

Search for rental destination regions by name
- **search_rentals**: Returns a list of matching rentals with pricing, amenities, and availability. Use this as the primary entry point for finding short-term rental properties.

Search vacation rentals across Expedia and Vrbo inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expedia Vrbo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a beachfront vacation home in Cancún for 8 guests, March 20-27."

**🤖 AI Agent:**
> I found 31 beachfront properties in Cancún for your dates. Top match: 'Villa Caribe' (ID: VR-82914) — 4 bedrooms, private pool, ocean view, $285/night ($1,995 total). Also strong: 'Casa del Sol' (ID: VR-19283) — 5 bedrooms, rooftop terrace, steps from the beach, $340/night ($2,380 total). Both have excellent guest ratings above 4.7. Want me to check the availability calendar or pull photos for either?

---

**👤 You:**
> "Show me the availability calendar for Villa Caribe through all of March."

**🤖 AI Agent:**
> Here's the March calendar for Villa Caribe (VR-82914): **Mar 1-8** — Available, $265/night. **Mar 9-14** — Booked. **Mar 15-19** — Available, $275/night. **Mar 20-27** — Available, $285/night (your requested dates). **Mar 28-31** — Available, $260/night. Minimum stay is 3 nights. Your Mar 20-27 window is still open. Would you like to proceed with booking?

---

**👤 You:**
> "Pull the photos for Villa Caribe so I can see what it looks like."

**🤖 AI Agent:**
> I've retrieved 24 photos for Villa Caribe (VR-82914). The gallery includes: exterior with infinity pool overlooking the Caribbean (main photo), 4 bedroom shots (all with ocean-facing windows), the open-plan kitchen with marble countertops, a rooftop lounge area, and 3 beach access views. The property looks exactly as described — modern construction with direct beach access. Want me to compare this visually against Casa del Sol as well?


## ❓ FAQ

**Q: Can my AI agent find entire homes for a group trip with specific amenities like a pool or hot tub?**
Yes. Use the `search_rentals` tool with your destination, dates, guest count, and amenity preferences. The agent will filter results to show only properties matching your criteria, including pricing per night and total stay cost. You can then drill into any listing with `get_rental_details` for the full amenity breakdown.

**Q: How can I check which dates a property is available before booking?**
The `get_rental_calendar` tool pulls the full availability calendar for any property. It shows open dates, blocked periods, nightly rates per date, and minimum stay requirements. Your agent can scan multiple weeks or months to identify the optimal booking window based on your budget and schedule.

**Q: Can I see photos of a rental property before making a decision?**
Yes. The `get_rental_images` tool returns the complete photo gallery for any property, including high-resolution images of bedrooms, living areas, kitchen, exterior, and amenities. Your agent can provide direct image URLs that you can preview in your browser or include in a planning document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia-vrbo](https://vinkius.com/mcp/expedia-vrbo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expedia Vrbo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `expedia-vrbo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expedia Vrbo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expedia-vrbo": {
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
