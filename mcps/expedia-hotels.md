# Expedia Hotels MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia-hotels)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/expedia-hotels-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/expedia-hotels-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate hotel research via Expedia — search global property availability, compare room rates, and analyze guest reviews directly from any AI agent.

## Description
Connect your **Expedia Rapid API** account to any AI agent and take programmatic control over one of the world's largest hotel inventory networks.

### What you can do

- **Property Search** — Scan thousands of hotels worldwide by location, dates, guest count, and star rating to find real-time availability
- **Rate Comparison** — Pull detailed rate plans for any property, comparing prices across room types, cancellation policies, and meal inclusions
- **Guest Reviews** — Extract aggregated review scores and recent guest feedback to make data-driven accommodation decisions
- **Itinerary Management** — Create, retrieve, and cancel hotel bookings programmatically through the Rapid API
- **Region Discovery** — Query destination suggestions and region metadata to power intelligent location-based searches

### How it works

1. Sign up at the [Expedia Group Developer Hub](https://developers.expediagroup.com/) and create a Rapid API project
2. Generate your API Key and Shared Secret from the portal
3. Enter your credentials here and start querying hotel inventories from Claude, Cursor, or any MCP-compatible client

No more switching between browser tabs to compare hotels. Your AI agent handles the deep search while you focus on the decision.

### Who is this for?

- **Corporate Travel Coordinators** — instantly search and compare hotel blocks near conference venues for large teams
- **Travel Agency Operators** — pull real-time rate plans and availability without navigating the consumer frontend
- **Revenue Analysts** — monitor pricing trends and competitor rates across markets programmatically


## Available Tools
- **book_hotel**: This is a write action that results in an actual reservation. Required fields: property_id, check_in_date, check_out_date, room_id, rate_plan_id, guest first name, last name, and email. The room_id and rate_plan_id should be obtained from the check_availability or get_rate_plans tools. Include billing address and special requests if the user provides them. On success, returns an itinerary ID that can be used to retrieve or cancel the booking. ALWAYS confirm booking details with the user before executing this action.

Book a hotel reservation through Expedia EAN
- **cancel_itinerary**: This is a write action that modifies a real reservation. Whether a refund is available depends on the cancellation policy of the specific rate plan that was booked. Some rate plans are non-refundable. ALWAYS confirm the cancellation with the user and inform them of the applicable cancellation policy before executing this action. Returns the updated itinerary with cancellation status and any refund details.

Cancel a hotel booking by itinerary ID
- **check_availability**: Returns available room types, bed configurations, occupancy limits, cancellation policies, and pricing. Use this after a user has identified a hotel of interest to see what rooms are available for their desired stay dates. Required: property_id, check_in_date, check_out_date.

Check room availability for a specific hotel property
- **check_price_match**: This is part of Expedia's price match guarantee program. Required: property_id, check_in_date, check_out_date, competitor_url (URL where the lower price was found), and competitor_price (the lower price amount). Returns the price match result including whether the match was approved, the adjusted price if applicable, and any refund or credit details.

Check if a hotel price matches a competitor's price
- **get_hotel_details**: Returns property name, full address, phone number, star rating, guest rating, detailed descriptions, amenities list, policies (check-in/out times, pet policy, etc.), nearby attractions, and images. Use this to present rich hotel details to the user before they make a booking decision.

Get detailed information about a specific hotel property
- **get_hotel_images**: Returns image URLs in various categories (exterior, lobby, room, bathroom, pool, restaurant, etc.), along with image descriptions, captions, and subject IDs. Use this to display hotel photos to the user when browsing or presenting hotel details. Images are available in multiple sizes — the response includes URLs for each size variant.

Get all images for a specific hotel property
- **get_itinerary**: Returns booking status (confirmed, cancelled), property details, room information, check-in/check-out dates, guest details, total price paid, cancellation policy, and booking timestamps. Use this to check the status of a booking or to present booking confirmation details to the user.

Get details of a hotel booking by itinerary ID
- **get_rate_plans**: This includes standard rates, member-only deals, package rates, non-refundable options, and promotional pricing. Each rate plan includes details on meal plans (room only, breakfast included), cancellation policies, payment types (pay now vs pay at property), and total pricing. Use this to compare pricing options and present the best deals to the user.

Get rate plans and pricing options for a hotel property
- **search_hotels**: Use this to find hotels by destination region ID, check-in and check-out dates, number of rooms and guests. You can filter by amenities, price range, star rating, guest rating, and property type. The region ID can be obtained using the search_regions tool. Always provide check-in and check-out dates in ISO format (YYYY-MM-DD). Results include property IDs, names, locations, star ratings, and pricing information.

Search for hotels using the Expedia EAN API
- **search_regions**: This is the first step in a hotel search — you need a region_id to search for hotels. For example, searching for "Paris" returns the city region, specific neighborhoods, and nearby airports. Use this to help the user identify the correct destination before performing a hotel search. Returns region IDs, names, types, and hierarchy info.

Search for destination regions by name
- **get_guest_reviews**: Returns individual review entries with ratings (overall, cleanliness, staff, comfort, location), review text, traveler type, travel dates, and submission dates. Use this to help the user evaluate a property based on real guest experiences before booking. You can filter by traveler type or sort by date or rating.

Get guest reviews and ratings for a specific hotel
- **price_check**: This is the recommended step between selecting a rate plan and creating a booking — it confirms the price is still valid, checks for any price changes, and returns the final confirmed amount including taxes and fees. Requires property_id, room_id (from check_availability), and rate_id (from get_rate_plans). If the price has changed, the response includes the updated pricing.

Validate the current price for a specific room and rate before booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expedia Hotels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find available 4-star hotels in central Paris for December 15-18, two adults."

**🤖 AI Agent:**
> I found 23 properties matching your criteria in central Paris. The top three are: 'Hôtel Le Marais' (ID: 28491) starting at €189/night with free cancellation, 'Grand Palais Suites' (ID: 74502) at €245/night including breakfast, and 'Opéra Garnier Hotel' (ID: 15893) at €210/night. Would you like me to pull the detailed rate plans for any of these?

---

**👤 You:**
> "Show me the cancellation policy and rate breakdown for property 28491."

**🤖 AI Agent:**
> Here are the rate plans for Hôtel Le Marais (28491): **Standard Room** — €189/night, free cancellation until Dec 13, total €567 + €42 taxes. **Superior Room** — €229/night, non-refundable, includes daily breakfast, total €687 + €51 taxes. The standard room offers the best flexibility. Want me to check guest reviews before you decide?

---

**👤 You:**
> "What are the latest guest reviews saying about property 74502?"

**🤖 AI Agent:**
> Grand Palais Suites (74502) has a 4.6/5.0 average from 892 reviews. Recent highlights: guests consistently praise the central location (50m from Champs-Élysées) and the included breakfast quality. The most common critique mentions elevator wait times during peak morning hours. Overall sentiment is strongly positive — 94% of recent reviewers recommend the property.


## Installation & Usage

To install and use the **Expedia Hotels** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia-hotels](https://vinkius.com/mcp/expedia-hotels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
