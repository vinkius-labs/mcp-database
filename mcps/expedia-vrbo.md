# Expedia Vrbo MCP Server

Automate vacation rental research via Vrbo — search entire homes, compare nightly rates, and check availability calendars directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia-vrbo)

## Overview
**Category:** ecommerce
**Tools Count:** 11

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


## Available Tools
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
- **get_unit_amenities**: Returns structured amenity data including categories (kitchen, bathroom, entertainment, outdoor, safety), individual amenity names, descriptions, and availability status. Use this when the user needs to verify specific amenities like pool, wifi, parking, pet-friendliness, or accessibility features.

Get the full list of unit amenities for a vacation rental
- **search_rental_regions**: Returns region IDs, names, types (city, neighborhood, airport, poi), and coordinates. Use this as a first step when the user provides a destination name instead of a destination_id, to resolve the name into a valid region ID for search_rentals.

Search for rental destination regions by name
- **search_rentals**: Returns a list of matching rentals with pricing, amenities, and availability. Use this as the primary entry point for finding short-term rental properties.

Search vacation rentals across Expedia and Vrbo inventory
- **get_rental_reviews**: Returns individual review entries with overall ratings, category scores (cleanliness, communication, location, value), review text, traveler name, travel dates, and submission dates. Use this to help the user evaluate a rental property based on real guest experiences. Especially useful for comparing properties or verifying quality before booking.

Get guest reviews and ratings for a vacation rental property


## Installation & Usage

To install and use the **Expedia Vrbo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia-vrbo](https://vinkius.com/mcp/expedia-vrbo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
