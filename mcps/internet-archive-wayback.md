# Internet Archive Wayback MCP Server

Check URL archival status, explore capture history, and analyze Wayback Machine data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive-wayback)

## Overview
**Category:** knowledge-management
**Tools Count:** 10

## Description
Connect the **Internet Archive Wayback Machine** to any AI agent and access the world's largest web archive — 800B+ archived web pages spanning 25+ years of internet history.

### What you can do
- **URL Availability Check** — Verify if any URL has been archived and find the latest snapshot
- **Full CDX Capture History** — Get detailed capture history with timestamps, status codes, MIME types, and sizes
- **Filter by Year** — Find all captures from a specific year for temporal analysis
- **Filter by HTTP Status** — Find captures that returned specific status codes (200, 404, 301, 500)
- **Filter by MIME Type** — Find captures of specific resource types (HTML, images, PDFs, CSS)
- **First Capture** — Find when a URL was first archived
- **Latest Capture** — Find the most recent archived version of a URL
- **Capture Count** — Get the total number of times a URL has been archived
- **Deduplicated Captures** — Get unique captures collapsed by URL key
- **Subdomain Discovery** — Find all archived subdomains of a domain

### How it works
1. Subscribe to this server
2. No API key needed — completely free and public
3. Start exploring web history from Claude, Cursor, or any MCP-compatible client

The Wayback Machine is a non-profit service preserving internet history — no authentication required for access.

### Who is this for?
- **Journalists & Researchers** — find archived versions of websites to verify claims, track content changes, and recover deleted information
- **Web Developers** — analyze how websites evolved over time, compare design changes, and find historical implementations
- **Legal & Compliance** — preserve evidence of website content at specific points in time for legal proceedings
- **Historians & Academics** — study the evolution of the internet, track how organizations presented themselves online over decades
- **Cybersecurity** — investigate phishing sites, track domain changes, and discover subdomain footprints


## Available Tools
- **get_captures_by_mime_type**: Common types: "text/html" (web pages), "image/jpeg" (JPEG images), "application/pdf" (PDFs), "text/css" (stylesheets). Use this to find specific resource types in the archive.

Get captures filtered by MIME type
- **get_captures_by_status**: Common codes: "200" (OK), "404" (Not Found), "301" (Redirect), "500" (Server Error). Use this to analyze site availability patterns over time.

Get captures filtered by HTTP status code
- **get_captures_by_year**: Use this to analyze archival frequency or find snapshots from a particular year. Year should be 4-digit format (e.g., "2020").

Get captures filtered by a specific year
- **get_cdx_captures**: Each capture includes timestamp, original URL, MIME type, HTTP status code, and file size. Use this for comprehensive archival analysis. Optional limit parameter controls maximum results.

Get detailed capture history from the CDX server
- **check_availability**: Returns the closest (most recent) snapshot timestamp and availability status. Use this to verify if a page is preserved and find its latest archived version.

Check if a URL has been archived by the Wayback Machine
- **get_captures_collapsed**: This shows unique page captures without redundant entries for the same page. Use this for a cleaner view of archived content.

Get captures deduplicated by URL key
- **get_capture_count**: Use this to measure how frequently a page has been preserved over time.

Get the total number of captures for a URL
- **get_first_capture**: Includes the timestamp, status code, and original URL. Use this to find when a page was first preserved.

Get the first (earliest) capture of a URL
- **get_latest_capture**: Includes timestamp, status code, and URL. Use this to find the newest preserved version of a page.

Get the most recent capture of a URL
- **get_subdomain_captures**: g., *.example.com). Use this to discover the archival footprint of an entire domain, finding all subdomains that have been preserved.

Get captures for all subdomains of a domain


## Installation & Usage

To install and use the **Internet Archive Wayback** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive-wayback](https://vinkius.com/mcp/internet-archive-wayback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
