# DataDome MCP Server

Equip your AI agent to monitor bot protection, track threats, and audit protected endpoints directly via the DataDome API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datadome)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Integrate **DataDome**, the leading bot protection and fraud prevention solution, directly into your AI workflow. Monitor your web and mobile applications for automated threats, audit protected endpoints, and track real-time protection statistics using natural language.

### What you can do

- **Threat Monitoring** — List and retrieve full details for recently detected bot threats and suspicious activities.
- **Endpoint Auditing** — Monitor the health and protection status of all your integrated web and mobile endpoints.
- **Protection Insights** — Access real-time statistics and dashboard data on bot traffic and mitigation.
- **Rule Management** — List custom bot rules and explore bypass tokens configured in your account.

### How it works

1. Connect the DataDome integration to your AI assistant.
2. Authorize using your DataDome Management API Key (found in your dashboard settings).
3. Manage your bot protection strategy through intuitive conversation.

### Who is this for?

- **Security Engineers** — Quickly check threat logs and verify endpoint protection status on the go.
- **SREs & DevOps** — Monitor application health and bot traffic trends via chat.
- **Fraud Analysts** — Gather structured data on recent bot activities and threat types for reporting.


## Available Tools
- **get_bot_traffic_summary**: Returns a summary of traffic from "Good Bots" (e.g., search engines) versus "Bad Bots" (e.g., scrapers, scrapers) and their impact on total traffic.

Get a summary of bot traffic categorized by type
- **get_endpoint_health**: Returns latency metrics, error rates, and the current operational state of the DataDome integration for the endpoint.

Check the health status of a specific protected endpoint
- **get_protection_stats**: Returns real-time counts of allowed vs. blocked requests, captcha pass rates, and identified bot categories.

Retrieve real-time protection statistics and dashboard data
- **get_threat_details**: Resolves detailed request headers, behavioral patterns, and the specific detection logic triggered.

Get full technical details for a specific threat ID
- **list_protected_applications**: Returns application names, API keys (masked), and the types of protection enabled (Web/Mobile/API).

List all applications (mobile, web) integrated with DataDome
- **list_protected_endpoints**: Returns metadata including endpoint URLs, protection status, and associated application IDs.

List all endpoints protected by DataDome
- **list_access_logs**: Returns a stream of recent requests processed by DataDome, including bot scores, decision outcomes, and geo-location data.

List recent access logs filtered by DataDome
- **list_custom_bot_rules**: Returns a list of custom bot detection rules, including match criteria (IP, User-Agent, etc.), action (allow/block/captcha), and rule priority.

List all custom blocking and allowing rules
- **list_recent_threats**: Returns a list of recent security incidents including threat types (e.g., scraping, credential stuffing), origin IPs, and detection timestamps.

List recently detected bot threats and suspicious activities
- **search_threats_by_type**: Matches the provided threat type against recent incidents to isolate specific attack vectors like "scraper" or "crawler".

Search for recent threats by threat type keyword


## Installation & Usage

To install and use the **DataDome** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadome](https://vinkius.com/mcp/datadome)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
