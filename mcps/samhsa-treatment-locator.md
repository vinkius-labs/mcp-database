# SAMHSA Treatment Locator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/samhsa-treatment-locator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/samhsa-treatment-locator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/samhsa-treatment-locator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Find substance use and mental health treatment facilities across the US using official SAMHSA locator data.

## Description
Connect to the **SAMHSA Treatment Locator** and empower your AI agent to find critical healthcare resources across the United States. This server provides direct access to the official Substance Abuse and Mental Health Services Administration database.

### What you can do

- **Geographic Search** — Find facilities using precise latitude and longitude coordinates within a customizable radius.
- **Service Filtering** — Narrow down results using specific service codes to find the exact type of care needed (e.g., detox, inpatient, outpatient).
- **Detailed Facility Profiles** — Retrieve comprehensive metadata for specific facilities, including contact information and available services via unique identifiers.
- **Service Code Discovery** — Access the full list of available service categories and codes to refine your searches effectively.

### How it works

1. Subscribe to this server
2. Enter your SAMHSA API Key
3. Start locating treatment centers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Coordinators** — quickly identify nearby treatment options for patients based on specific clinical needs.
- **Public Health Researchers** — analyze the distribution of mental health and substance use services in specific regions.
- **Social Workers** — find and inspect facility details directly from their workflow tools to assist clients faster.


## Available Tools
- **get_facility**: Get detailed information for a specific facility
- **list_services**: List available service codes used for filtering
- **search_facilities**: Search for treatment facilities based on location and filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAMHSA Treatment Locator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for treatment facilities within 25 miles of latitude 34.05 and longitude -118.24."

**🤖 AI Agent:**
> I found several facilities near Los Angeles. The closest ones include 'Central Recovery Center' and 'Hope Health Services'. Would you like the details for any of these?

---

**👤 You:**
> "Get the full details for facility ID 'FAC123456'."

**🤖 AI Agent:**
> Retrieving details for FAC123456... This is the 'Evergreen Wellness Center' located at 123 Main St. They offer outpatient mental health services and specialized youth programs.

---

**👤 You:**
> "List all available service codes for filtering treatment searches."

**🤖 AI Agent:**
> I've compiled the service codes. Categories include 'Substance Use' (codes: DETOX, RES), 'Mental Health' (codes: OP, IP), and 'Special Programs' (codes: VET, LGBTQ). Which category should we filter by?


## Installation & Usage

To install and use the **SAMHSA Treatment Locator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/samhsa-treatment-locator](https://vinkius.com/mcp/samhsa-treatment-locator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
