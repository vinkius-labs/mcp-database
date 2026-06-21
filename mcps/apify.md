# Apify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Command Apify scrapers from your AI agent — run actors, extract web data, poll datasets, and automate browser tasks seamlessly.

## Description
Connect your **Apify** workspace to your AI agent and seamlessly direct full-stack web scraping and data extraction workflows through natural conversation.

### What you can do

- **Discover & Run Actors** — Browse all scraper bots (Actors) available in your account. Fire them off asynchronously or synchronously for fast, targeted scraping
- **Extract Datasets** — Pull robust structured data formats out of completed runs. Retrieve detailed JSON records directly into the agent's context window
- **Fetch Key-Value Stores** — Programmatically read snapshots, cached HTML pages, or screenshots from the Apify Key-Value repositories mapped to a run
- **Job Control & Scalability** — Stop hanging scraper jobs, queue new dynamic URLs mid-run, or inspect deep usage analytics, compute units, and webhooks limits

### How it works

1. Subscribe to this server
2. Enter your Personal Apify API Token
3. Start exploring and interacting with data extraction routines securely via Claude or Cursor

### Who is this for?

- **Data Engineers** — trigger scheduled extraction logic seamlessly and map Apify objects within a conversational QA check
- **Market Researchers** — command the AI to scrape product prices using Apify actors and compile the JSON datasets into readable markdown tables
- **AI Developers** — augment your agent's real-time capabilities by feeding it massive structured site data freshly scraped via headless browsers


## Available Tools
- **abort_run**: Any data already scraped and pushed to the dataset is preserved. The run status changes to ABORTED. Use this to stop runaway scrapes or when sufficient data has been collected. Graceful shutdown depends on the actor implementation.

Abort an active Apify actor run
- **get_account_limits**: Essential for monitoring consumption and avoiding overage charges.

Check Apify account subscription limits and compute unit usage
- **get_dataset_items**: The datasetId is found in the run object (defaultDatasetId). Supports pagination via limit (max items per page) and offset (starting position). Returns an array of JSON objects containing the scraped data fields. Use limit=1000 for bulk downloads.

Export structured JSON data from an Apify dataset
- **get_key_value_store**: Key-value stores hold arbitrary data like screenshots (OUTPUT), configuration files, or intermediate results. The storeId comes from the run object (defaultKeyValueStoreId). Common keys include "OUTPUT", "INPUT", and "SCREENSHOT".

Retrieve an item from an Apify actor key-value store
- **get_run**: Poll this endpoint to track long-running scrapes.

Check the status and metadata of a specific Apify actor run
- **list_actors**: Includes owned actors and those from the Apify Store that have been saved. Each entry contains the actorId, name, description, and default run configuration. Use the actorId to trigger runs.

List all accessible actors in the Apify account
- **list_webhooks**: RUN.SUCCEEDED, ACTOR.RUN.FAILED), target URLs, and associated actor IDs. Webhooks enable event-driven architectures by notifying external systems when actor runs complete or fail.

List all configured webhooks in the Apify account
- **push_to_queue**: Pass the queueId (from the run object) and a JSON string array of request objects, e.g., [{"url":"https://...","uniqueKey":"..."}]. This enables dynamic crawling where new pages are discovered and added during execution.

Dynamically push new URLs to an active Apify request queue
- **run_actor_sync**: run_actor but waits for the actor to finish before returning. The response includes the full run object with defaultDatasetId for immediate data retrieval. Best for short-lived actors (under 5 minutes). For long-running scrapes, use the async ap.run_actor instead.

Run an Apify actor and block until completion (synchronous)
- **run_actor**: Pass the actorId (e.g., "apify/web-scraper" or a custom ID) and a JSON string with the input configuration (start URLs, proxy settings, max pages, etc.). Returns immediately with a runId. Use ap.get_run to poll for completion and ap.get_dataset_items to retrieve extracted data.

Start an Apify actor asynchronously with custom JSON input


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the Apify actors available on my account."

**🤖 AI Agent:**
> I've scanned your Apify actor catalog. You possess 3 main actors: 'ecommerce-spider-v1' and two public templates 'google-search-scraper' and 'instagram-scraper'. Shall I print their base configurable inputs?

---

**👤 You:**
> "Verify the status of run 'qKpwH9LgC3r0Xm' and show me its final dataset if finished."

**🤖 AI Agent:**
> I checked run `qKpwH9LgC3r0Xm`. Its current status is `SUCCEEDED`. The run consumed 0.045 Compute Units. I have successfully downloaded the associated dataset (`ds_8aBxP_...`) which yielded 302 product profiles. I'm injecting the top 5 parsed items below.

---

**👤 You:**
> "How are our compute usage limits tracking this current month on Apify?"

**🤖 AI Agent:**
> I pulled your overall compute records. Right now on the 'Scale' plan, your account used 82 out of 100 Compute Units (CU). You've consumed significant resources on proxy bandwidth (1.8TB/2TB) leading to roughly 80% usage threshold. I recommend holding further massive scraped runs until renewal happens on the 10th.


## Installation & Usage

To install and use the **Apify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apify](https://vinkius.com/mcp/apify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
