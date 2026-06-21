# TollGuru MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tollguru)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tollguru-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tollguru-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate tolls and trip costs via TollGuru — get toll plaza details, fuel costs, and route optimization for any route across 50+ countries from any AI agent.

## Description
Connect your **TollGuru** toll calculation API to any AI agent and take full control of trip cost estimation, toll plaza tracking, route optimization, and fleet expense management across 50+ countries through natural conversation.

### What you can do

- **Toll Calculation** — Calculate toll costs for any route with detailed plaza-by-plaza breakdown including tag and cash prices
- **Fuel Cost Estimation** — Get fuel cost estimates based on vehicle efficiency and current fuel prices along the route
- **Driver Cost Analysis** — Calculate driver costs based on hourly wage or time value for complete trip budgeting
- **Multi-Stop Routes** — Calculate tolls for routes with multiple waypoints and optimize waypoint order to minimize tolls
- **Route Optimization** — Find the most cost-effective route between origin and destination with toll-aware routing
- **Polyline Toll Calculation** — Calculate tolls for existing routes from Google Maps, Here Maps, or Mapbox polylines
- **Vehicle-Specific Pricing** — Get accurate toll costs for any vehicle type from 2-axle cars to 9-axle commercial trucks
- **Multi-Currency Support** — View costs in USD, CAD, MXN, EUR, GBP, INR, AUD, and 12+ other currencies
- **Payment Method Breakdown** — Compare toll costs by payment method (tag, cash, prepaid card, license plate)
- **Global Coverage** — Calculate tolls across US, Canada, Mexico, Europe, Australia, India, and 50+ countries

### How it works

1. Subscribe to this server
2. Enter your TollGuru API key (free tier: 150 transactions/day with corporate email)
3. Start calculating toll costs from Claude, Cursor, or any MCP-compatible client

No more manually checking toll authority websites or estimating trip costs. Your AI acts as a dedicated toll analyst and trip budgeting assistant.

### Who is this for?

- **Fleet Managers** — calculate toll costs for delivery routes, optimize waypoint order, and manage trip expenses
- **Road Trippers** — estimate total trip costs including tolls, fuel, and driver time before heading out
- **Logistics Planners** — compare toll costs across route options and select the most cost-effective paths
- **Travel Budgeters** — get comprehensive cost breakdowns for any road trip with toll, fuel, and time costs


## Available Tools
- **calculate_toll_multi_stop**: Returns detailed breakdown of tolls at each plaza along the complete route, fuel costs, and optional driver costs. Supports waypoint optimization to minimize total toll costs. Essential for delivery route planning, multi-stop trip budgeting, and logistics optimization. AI agents should use this when users need toll calculations for routes with multiple stops, such as "calculate tolls from Chicago to Detroit with stops in Toledo and Ann Arbor" or "what are the toll costs for my delivery route with 5 waypoints".

Calculate tolls for a multi-stop route with multiple waypoints
- **calculate_toll_from_polyline**: This is useful when you already have a route from a mapping service and need toll calculations without re-routing. Returns the same detailed toll, fuel, and cost information as the route calculation. Supports all vehicle types, currencies, and payment methods. Essential for integrating with existing mapping applications, post-trip toll reconciliation, and GPS track-based toll analysis. AI agents should use this when users have an existing route polyline from Google Maps, Here Maps, or another service and need toll costs for that specific route.

Calculate tolls for a route defined by an encoded polyline from any mapping service
- **calculate_toll_route**: Returns detailed toll plaza information including plaza names, tag and cash costs, payment methods accepted, and route optimization suggestions. Also calculates fuel costs based on vehicle efficiency and current fuel prices, and optional driver costs based on time value. Supports all vehicle types including 2-axle cars, EVs, motorcycles, and commercial trucks (2-9+ axles). You can request route optimization to minimize toll costs, specify currency output (USD, CAD, MXN, EUR, GBP, INR, AUD, etc.), and choose mapping service (Here Maps, Google Maps, or TollGuru internal). Essential for fleet management, trip cost estimation, route planning, toll reconciliation, and travel budgeting. AI agents should use this when users ask "what are the tolls from New York to Boston", "calculate toll costs for my truck from LA to San Francisco", or need comprehensive trip cost breakdowns including tolls, fuel, and driver time.

Calculate tolls and total trip costs for a route with origin, destination, and optional waypoints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TollGuru** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate toll costs for a car trip from San Francisco to Los Angeles."

**🤖 AI Agent:**
> Calculating toll costs for San Francisco to Los Angeles... Route distance: 383 miles, estimated drive time: 5h 45m. Toll plazas: Bay Bridge ($7.00 tag / $8.00 cash). Total toll cost: $7.00 with FasTrak tag, $8.00 cash. Estimated fuel cost: $42.50 (25 mpg vehicle, $3.50/gal). Total trip cost: $49.50-$50.50. Alternative routes available via I-5 (no tolls, longer distance) or CA-101 (scenic, similar tolls). Would you like a comparison of all route options?

---

**👤 You:**
> "What are the toll costs for a 5-axle truck from Chicago to Detroit?"

**🤖 AI Agent:**
> Calculating toll costs for 5-axle truck Chicago to Detroit... Route distance: 283 miles, estimated drive time: 4h 30m. Toll plazas: Chicago Skyway ($8.40 tag / $9.60 cash), Indiana Toll Road I-80/I-90 ($22.50 tag / $26.80 cash). Total toll cost: $30.90 with tag, $36.40 cash. Estimated fuel cost: $98.00 (6 mpg truck, $4.20/gal diesel). Estimated driver cost: $135.00 (at $30/hour). Total trip cost: $263.90-$269.40. Would you like alternative routes with lower toll costs?

---

**👤 You:**
> "Optimize a delivery route with stops in Philadelphia, Baltimore, and Washington DC starting from New York."

**🤖 AI Agent:**
> Optimizing multi-stop route... Original order: New York → Philadelphia → Baltimore → Washington DC. Optimized order (lowest tolls): New York → Baltimore → Washington DC → Philadelphia. Total distance: 287 miles. Toll plazas: NJ Turnpike ($13.85 tag), Baltimore Harbor Tunnel ($4.00 tag), I-95 Delaware Memorial Bridge ($5.00 tag). Total optimized toll cost: $22.85 with tag, $28.25 cash. Savings from optimization: $6.40 in tolls. Fuel cost: $38.50. Total trip cost: $61.35-$66.75. Would you like detailed waypoint-by-waypoint breakdown?


## Installation & Usage

To install and use the **TollGuru** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tollguru](https://vinkius.com/mcp/tollguru)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
