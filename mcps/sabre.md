# Sabre MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sabre)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Search and book flights and hotels globally using Sabre's travel technology platform — access Bargain Finder Max and PNR management.

## Description
Connect your **Sabre** developer account to any AI agent and manage global travel bookings through natural conversation.

### What you can do

- **Flight Shopping** — Search for the lowest available fares using the Bargain Finder Max engine for any route and date range.
- **PNR Creation** — Create Passenger Name Records (PNR) for flights, combining selection, passenger data, and payment.
- **Hotel Search** — Query global hotel inventories based on location, dates, and specific guest criteria.
- **Property Intelligence** — Retrieve detailed information about specific hotels, including amenities, policies, and descriptions.
- **Hotel Booking** — Finalize hotel reservations with integrated guest and payment details.

### How it works

1. Subscribe to this server
2. Enter your Sabre Client ID and Client Secret
3. Start searching and booking travel from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agencies** — automate the search and booking process for clients using AI-driven workflows
- **Corporate Travel Managers** — quickly find and compare flight options and hotel availability for team trips
- **Travel App Developers** — test and integrate Sabre's core travel services directly from the development environment


## Available Tools (5)
- **book_hotel**: The payload is a CreatePassengerNameRecordRQ object for a hotel segment. Top-level shape:
{ "CreatePassengerNameRecordRQ": { "TravelItineraryAddInfoRQ": { ... }, "HotelContent": { ... }, "PaymentInfo": { ... } } }

TravelItineraryAddInfoRQ carries "AgencyInfo", "CustomerInfo" (array of "PersonName" and contact "Email"/"Phone") and "TravelItineraryRef". HotelContent holds the selected room/rate taken from the price-checked search result. PaymentInfo carries the "PaymentCard" (CardType, CardNumber, ExpiryMonth/ExpiryYear, SecurityCode).

This is a state-changing action that creates a real hotel reservation. Confirm traveler names, room selection, cancellation policy and payment with the user before calling.

Book a hotel reservation
- **create_booking**: The payload is a CreateBookingRQ object. Top-level shape:
{ "CreateBookingRQ": { "BookedFlight": { ... }, "Travelers": [ ... ], "FormOfPayment": { ... }, "PostProcessing": { ... } } }

BookedFlight comes from the price-check/revalidate response of shop_flights. Travelers is an array of objects with "PersonName" (given "First" and sur "Last") plus contact "Email" and "Phone". FormOfPayment requires a "PaymentCard" with "CardType" (e.g. "VI"), "CardNumber", "ExpiryMonth"/"ExpiryYear" and "SecurityCode".

This is a state-changing action: it creates a real PNR in the Sabre environment configured (cert or prod). Always confirm the traveler names and payment details with the user before calling.

Create a Passenger Name Record (PNR) for a flight
- **get_hotel_details**: The payload is a GetHotelDetailsRQ object. Top-level shape:
{ "GetHotelDetailsRQ": { "SearchCriteria": { "HotelRefs": [ { "HotelCode": "1002345" } ] } } }

HotelCode comes from the "HotelAvailInfo" array of search_hotels, or can be looked up by name/city through that same search. Multiple HotelRefs can be sent in one call. The response carries "HotelInfo" with "Amenities", "Descriptions", "Policies" (including cancellation and check-in/out rules), "ContactInfo" and "MediaInfo".

Use this after search_hotels to narrow down a property before booking; it does not return live rates.

Get detailed information about a specific hotel
- **search_hotels**: The payload is a GetHotelAvailRQ object. Top-level shape:
{ "GetHotelAvailRQ": { "POS": { "Source": { "PseudoCityCode": "..." } }, "SearchCriteria": { "GeoSearch": { ... }, "StayDateTimeRange": { "StartDate", "EndDate" }, "RoomInfo": { ... } } } }

StayDateTimeRange uses ISO dates (StartDate "2026-06-01", EndDate "2026-06-05"). Location is set through GeoSearch: either "GeoRef" with "Radius" plus a "Address" / "GeoCoordinates" point, or a "HotelCityCode" / "CountryCode" inside "SearchCriteria". RoomInfo takes "GuestCount" entries (a "Count" per "AgeQualifyingCode": ADT=adult, CHD=child) and "RoomCount".

Response includes a "HotelAvailInfo" array with hotel codes, names, rates and a "SearchCacheKey" used by get_hotel_details. Rates shown are the lead rate and may change at price-check time.

Search for hotels globally
- **shop_flights**: The payload is a BargainFinderMaxRQ object. Top-level shape:
{ "OTA_AirLowFareSearchRQ": { "OriginDestinationInformation": [ ... ], "TravelerInfo": { ... }, "TPA_Extensions": { ... } } }

Each OriginDestinationInformation entry needs "OriginLocation" (IATA code), "DestinationLocation" (IATA code), "DepartureDateTime" (ISO, e.g. "2026-12-10T00:00:00"), and for round trips a second entry with "ReturnDateTime" or a "RPH" of 2. TravelerInfo needs "AirTraveler" entries with a numeric "TravelerTypeCode" (ADT=adult, CHD=child, INF=infant) and "PassengerTypeQuantity".

Dates are in the traveler's local airport time. Use IATA airport codes (JFK, LHR, CDG), never city names. The response contains priced itineraries grouped by slice; fares are not guaranteed until revalidated.

Search for lowest available flight fares (Bargain Finder Max)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sabre** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the cheapest flights from JFK to LHR departing on December 10th and returning on December 20th."

**🤖 AI Agent:**
> I'm searching via `shop_flights`... I found a round-trip option for $540 with British Airways. Would you like to see the full itinerary details?

---

**👤 You:**
> "Find available hotels in Paris for two adults from June 1st to June 5th."

**🤖 AI Agent:**
> Executing `search_hotels` for Paris... I've found 12 properties available. Top results include 'Hotel Lumiere' and 'Le Parisien'. Should I get the details for one of these?

---

**👤 You:**
> "Get the amenities and cancellation policy for hotel ID 1002345."

**🤖 AI Agent:**
> Fetching data via `get_hotel_details`... This property offers free Wi-Fi, a fitness center, and a pool. The cancellation policy requires 24-hour notice for a full refund.


## ❓ FAQ

**Q: How can I find the lowest available flight fares for a specific route?**
You can use the `shop_flights` tool. It utilizes Sabre's Bargain Finder Max API to return the lowest available fares based on your origin, destination, and date parameters.

**Q: Can I retrieve specific amenities and check-in policies for a hotel?**
Yes, the `get_hotel_details` tool allows you to fetch full metadata, including amenities, property descriptions, and operational policies for any specific hotel property.

**Q: Does this server support creating a full booking for a passenger?**
Absolutely. Use the `create_booking` tool for flights or `book_hotel` for accommodations to generate confirmed reservations with passenger and payment information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sabre](https://vinkius.com/en/ai-agent-connect/sabre)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sabre** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sabre` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sabre** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sabre": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
