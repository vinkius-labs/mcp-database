# TollGuru MCP Server

Global toll intelligence — calculate costs by address, coordinates, polyline, or GPS tracks with fuel estimates and multi-vehicle support.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tollguru-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Equip your AI agent with the most accurate toll intelligence available via **TollGuru**. This unified server provides your agent with instant access to toll costs, fuel consumption estimates, and route optimization for thousands of roads worldwide. Your agent can instantly calculate the total cost of a journey, audit individual toll booth prices, and suggest the most cost-effective path without you ever checking a map or calculator manually. Whether you are planning long-haul logistics or optimizing a personal road trip, your agent acts as a dedicated travel cost analyst through natural conversation.

### What you can do

- **Cost Calculation** — Calculate exact toll costs for any route between two or more addresses.
- **Vehicle Optimization** — Specify different vehicle types (Auto, Taxi, Truck) to get tailored pricing and technical details.
- **Route Auditing** — Fetch detailed summaries of individual toll charges and payment methods (Tag, Cash).
- **Logistics Intelligence** — Analyze total journey costs including fuel and tolls to optimize organizational planning.
- **Global Coverage** — Access toll data for thousands of bridges, tunnels, and highways across the globe.

### How it works

1. Subscribe to this server
2. Enter your TollGuru API Key
3. Start managing your travel intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Supply Chain Managers** — instantly retrieve exact shipping costs and optimize routes for fleet efficiency.
- **Travelers & Road Trippers** — plan their budgets accurately by knowing toll and fuel costs in advance.
- **Delivery & Ride-share Drivers** — audit daily expenses and find the most profitable routes through natural language.
- **SaaS Developers** — integrate complex toll and route pricing into their applications via an AI-guided interface.
- **Financial Controllers** — monitor corporate travel expenses and verify individual toll receipts.


## Available Tools
- **calculate_tolls_by_address**: Supports multiple vehicle types.

Calculate tolls and fuel costs between two addresses
- **calculate_tolls_by_coordinates**: Returns multiple route options with toll breakdowns.

Calculate tolls between two GPS coordinate pairs
- **calculate_tolls_by_gps**: Handles map-matching automatically for accurate toll identification from real trip data.

Calculate tolls from GPS track data (post-trip reconciliation)
- **calculate_tolls_by_polyline**: Submit the encoded polyline string to get toll costs for that exact path.

Calculate tolls for an encoded route polyline
- **get_toll_rates**: Look up toll rates for a specific toll plaza or booth
- **get_transaction_count**: Useful for monitoring usage and billing.

Get total API transaction count for your account


## Installation & Usage

To install and use the **TollGuru** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tollguru-alternative](https://vinkius.com/mcp/tollguru-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
