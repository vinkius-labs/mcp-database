# American Airlines MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/american-airlines)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/american-airlines-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/american-airlines-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI flight tracking: check flight status, schedules, and airport info via agents.

## Description
### What you can do

Connect AI agents to the American Airlines API for real-time flight tracking and airport information:

- **Track Flight Status** in real-time (On Time, Delayed, Cancelled) for any AA flight
- **View Flight Schedules** between any two airports served by American Airlines
- **Get Airport Info** including terminal layouts and available services
- **Plan Travel** by comparing schedules and finding alternative flights

### How it works

1. **Get your API key** from the [American Airlines Developer Portal](https://developer.aa.com/)
2. **Ask your AI agent** to check flight status, view schedules, or get airport details
3. **Natural language commands** replace manual app navigation
4. **Real-time data** directly from AA's operational systems

### Who is this for?

Essential for **frequent travelers**, **travel agents**, **airport staff**, and **flight enthusiasts**. Let AI agents monitor flight delays, plan trips by comparing schedules, and provide terminal information. Perfect for anyone flying American Airlines who wants instant status updates and schedule visibility through natural language.


## Available Tools
- **get_airport_info**: Useful for checking terminal layouts or finding specific amenities at a hub airport.

Get information about an airport served by American Airlines
- **get_flight_schedule**: Returns flight numbers, departure/arrival times, aircraft types, and service classes. Use this to plan travel, find alternative flights if one is full, or compare schedule options.

Get flight schedule between two airports on a specific date
- **get_flight_status**: Use this to track your flight, check on a relative's arrival, or monitor delays. Requires flight number (e.g., 123 or AA123) and date (YYYY-MM-DD).

Get real-time status of a specific American Airlines flight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **American Airlines** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of flight AA100 from JFK to LHR today"

**🤖 AI Agent:**
> I'll pull the real-time status and gate information for flight AA100.

---

**👤 You:**
> "Show me all flights from Miami to Dallas tomorrow morning"

**🤖 AI Agent:**
> I'll list the flight schedule for MIA to DFW for tomorrow.

---

**👤 You:**
> "What terminals are available at Chicago O'Hare (ORD)?"

**🤖 AI Agent:**
> I'll get the terminal information and services for ORD airport.


## Installation & Usage

To install and use the **American Airlines** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/american-airlines](https://vinkius.com/mcp/american-airlines)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
