# TollGuru MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tollguru-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tollguru-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tollguru-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Global toll intelligence — calculate costs by address, coordinates, polyline, or GPS tracks with fuel estimates and multi-vehicle support.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TollGuru** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate tolls from New York to Philadelphia for a standard car."

**🤖 AI Agent:**
> Retrieving route costs from NYC to Philly... For a 2-axle auto, the total toll cost is approximately $25.50 using a tag or $32.00 in cash. I can list the individual tolls like the Holland Tunnel and NJ Turnpike.

---

**👤 You:**
> "What is the cheapest route from San Francisco to Los Angeles considering tolls?"

**🤖 AI Agent:**
> Analyzing routes between SF and LA... I've found a path with zero tolls taking the I-5 S, though it may take slightly longer. The alternative route via the coastal highway has $15 in bridge tolls. Which one do you prefer?

---

**👤 You:**
> "How much does a 5-axle truck pay in tolls from Chicago to Miami?"

**🤖 AI Agent:**
> Fetching heavy vehicle rates for the Chicago-Miami corridor... For a 5-axle truck, the total estimated toll cost is $145.00. I have the breakdown of state-by-state charges and tag vs cash options ready for you.


## Installation & Usage

To install and use the **TollGuru** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tollguru-alternative](https://vinkius.com/mcp/tollguru-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
