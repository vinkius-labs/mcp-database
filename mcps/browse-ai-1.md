# Browse AI MCP Server

Automate web scraping with Browse AI — run extraction robots, monitor page changes, and retrieve bulk data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/browse-ai-1)

## Overview
**Category:** data-management
**Tools Count:** 10

## Description
Connect your **Browse AI** account to any AI agent and take full control of your no-code web scraping operations through natural conversation.

### What you can do

- **Robot Discovery** — List all your trained extraction and monitoring robots along with their configuration details
- **Execute Scrapes** — Trigger specific robots to run tasks on target URLs without lifting a finger
- **Data Retrieval** — Instantly download the final extracted JSON data from any successfully completed task
- **Bulk Operations** — Initiate multi-URL concurrent extractions and download the unified bulk datasets
- **Monitor Sync** — Check the status of your active web change monitors
- **Quota Management** — Retrieve your current API credits usage and monthly plan limits

### How it works

1. Subscribe to this server
2. Enter your Browse AI Secret API Key
3. Start fetching live data via Claude, Cursor, or any MCP-compatible client

No more manual downloads or periodic checks. Your AI agent serves as your pipeline to live web intelligence.

### Who is this for?

- **Data analysts** — pull massive datasets from recent bulk tasks straight into your agent for immediate processing
- **Marketers & SEO** — execute scraping robots on competitor URLs to generate instant market reports
- **Researchers** — extract complex targeted metrics without opening any third-party dashboards
- **Developers** — verify robot configurations, monitor credit usage, and inspect JSON payloads rapidly


## Available Tools
- **run_bulk_task**: Each set typically contains a different "originUrl". All extractions run concurrently on Browse AI infrastructure.

Run a Browse AI robot in bulk mode across multiple URLs
- **download_bulk_data**: Returns a JSON array where each element contains the capturedData from one task.

Download all extracted results from a completed Browse AI bulk run
- **get_bulk_task**: Get bulk task execution status from Browse AI
- **get_robot**: Get detailed configuration of a specific Browse AI robot
- **get_task_data**: Only meaningful when the task status is "successful". Fields match the column names configured in the Browse AI robot builder hitting internal task references.

Retrieve the final extracted JSON data from a successful Browse AI task
- **get_task**: Check the status of a specific Browse AI extraction task
- **list_credits**: Check Browse AI quota limits and credit usage
- **list_monitors**: Monitors run on scheduled intervals to detect changes on target web pages and trigger notifications or data captures automatically via `/monitors`.

List all active Browse AI web monitoring robots
- **list_robots**: Each robot represents a no-code AI scraping workflow targeting a specific website or data pattern via `GET /robots`.

List all Browse AI extraction and monitoring robots
- **run_robot**: Pass a JSON string of input parameters (typically including "originUrl" for the target page and any variable fields the robot expects). Returns a taskId.

Trigger a Browse AI robot to extract data from a target URL


## Installation & Usage

To install and use the **Browse AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browse-ai-1](https://vinkius.com/mcp/browse-ai-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
