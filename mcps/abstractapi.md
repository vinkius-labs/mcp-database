# AbstractAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abstractapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/abstractapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/abstractapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent with AbstractAPI's data enrichment — validate emails, geolocate IPs, check phone numbers, and enrich company data.

## Description
Connect your **AbstractAPI** account to your AI agent and unlock a powerful suite of data enrichment and validation utilities directly within your conversations. Stop writing disjointed scripts and let your agent handle data hygiene effortlessly.

### What you can do

- **Validate Contact Data** — Check email deliverability (MX records, disposable domains) and validate international phone numbers for carrier and line type
- **IP Geolocation** — Pass any IPv4 or IPv6 address and instantly retrieve the associated country, city, ISP, timezone, and local currency
- **Company Enrichment** — Look up any domain (e.g. google.com) and retrieve the company name, industry, headcount, and LinkedIn profile
- **Business Operations** — Fetch live currency exchange rates, validate EU VAT numbers, find public holidays for any country, or get precise timezone data
- **Media Utilities** — Generate UI avatars from names or render full-page website screenshots on the fly

### How it works

1. Subscribe to this server
2. Enter your precise AbstractAPI Key
3. Start verifying and enriching data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth & Sales teams** — build clean lists by asking your agent to enrich domains and validate scraped emails immediately
- **Developers & DevOps** — debug geographic routing quickly by having your agent geolocate IPs from your error logs
- **Financial Operators** — validate B2B EU VAT numbers and ask for real-time exchange rates in a single prompt


## Available Tools
- **geolocate_ip**: abstractapi.com. Pass an IPv4 or IPv6 address. Returns country, city, region, ISP, timezone, and currency data. Validates the key is for Geolocation.

Geolocate an IP address
- **validate_email**: abstractapi.com. Returns deliverability score, MX records check, and SMTP verification to ensure the inbox exists before sending.

Validate an email address
- **validate_phone**: abstractapi.com. Pass full phone number with country code. Returns carrier, line type (mobile/landline), and validity status.

Validate a phone number
- **enrich_company**: abstractapi.com. Pass a domain (e.g. google.com). Returns company name, industry, employee count, and LinkedIn profile link.

Enrich company data by domain
- **exchange_rate**: abstractapi.com. Returns the real-time or historical exchange rate between a base currency and a target currency.

Get live currency exchange rates
- **validate_vat**: abstractapi.com. Pass the VAT number with country prefix. Returns validity, company name, and registered legal address for B2B billing.

Validate an EU VAT number
- **list_holidays**: abstractapi.com. Pass ISO country code and year. Returns array of official local and national public holidays.

List public holidays for a country
- **get_timezone**: abstractapi.com. Pass city name or coordinates. Returns timezone name, UTC offset, and the exact current local time.

Get timezone data for a location
- **generate_avatar**: abstractapi.com. Returns a URL rendering an initials-based avatar image placeholder.

Generate an avatar image URL from a name
- **website_screenshot**: abstractapi.com. Returns a permanent URL rendering a full-page headless browser screenshot of the target website.

Capture a website screenshot URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AbstractAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if this email is safe to send to: john.doe@example.com?"

**🤖 AI Agent:**
> I've analyzed john.doe@example.com. It is NOT safe to send. The domain 'example.com' has no valid MX records and the SMTP handshake failed. Additionally, the quality score is 0.01 out of 1.0. This is likely a bounce trap.

---

**👤 You:**
> "Find out details about the IP address 8.8.8.8."

**🤖 AI Agent:**
> The IP address 8.8.8.8 is located in the United States. It's operated by the ISP 'Google LLC'. The exact timezone registered for this node is America/Los_Angeles, using the USD currency.

---

**👤 You:**
> "Enrich the company data for 'stripe.com'."

**🤖 AI Agent:**
> Stripe (stripe.com) operates in the Financial Services / FinTech sector. They were founded in 2010. They employ thousands globally and you can view their main corporate page here: linkedin.com/company/stripe.


## Installation & Usage

To install and use the **AbstractAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abstractapi](https://vinkius.com/mcp/abstractapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
