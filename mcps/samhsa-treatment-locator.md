# SAMHSA Treatment Locator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/samhsa-treatment-locator)
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


## ❓ FAQ

**Q: How can I search for treatment facilities near a specific set of coordinates?**
Use the `search_facilities` tool by providing the `lat` (latitude) and `lon` (longitude) parameters. You can also specify a `radius` in miles to define the search area.

**Q: Where can I find the list of service codes to filter my search?**
You can run the `list_services` tool. It will return all available service categories and their corresponding codes which you can then use in the `service_code` parameter of `search_facilities`.

**Q: Can I get the full contact information for a specific facility if I have its ID?**
Yes! Use the `get_facility` tool with the `facility_id`. This will retrieve detailed information including the address, phone number, and the full list of services provided by that location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/samhsa-treatment-locator](https://vinkius.com/mcp/samhsa-treatment-locator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAMHSA Treatment Locator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `samhsa-treatment-locator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAMHSA Treatment Locator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "samhsa-treatment-locator": {
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
