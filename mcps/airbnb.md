# Airbnb MCP Server

Search and manage Airbnb listings, experiences, reservations, and pricing directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/airbnb)

## Overview
**Category:** industry-titans
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **Airbnb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airbnb](https://vinkius.com/mcp/airbnb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
