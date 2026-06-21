# Routific MCP Server

Connect your AI assistant to Routific to solve complex vehicle routing problems, dispatch drivers, and manage global delivery timelines natively through chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/routific)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your conversational assistant directly to **Routific**, a premier logistics scaling platform. This integration seamlessly turns your AI into an advanced delivery dispatcher, allowing you to build multi-stop route solutions securely, manage outstanding delivery jobs, and proactively push dispatch tasks directly to drivers' mobile apps natively in one window.

### What you can do

- **Automate VRP Computations** — Submit basic logistics parameters (`solve_standalone_vrp`) or delegate massive multi-depot configurations organically (`solve_async_vrp_long`) and query asynchronous status returns effortlessly (`poll_async_solution`).
- **Control Saas Delivery Jobs** — Tell the AI to actively audit outstanding orders (`list_platform_jobs`) or create fresh delivery injections accurately handling order constraints and priorities directly into the system (`create_saas_job`, `update_saas_job`).
- **Assemble & Publish Timelines** — Review the resulting stop-by-stop ETAs securely calculated by algorithms natively inside the interface (`get_route_timeline`). Once completely satisfied, simply push the finalized route natively to the targeted driver's phone with an organic command (`publish_route_to_driver`).

### How it works

1. Install the Routific operations module into your active MCP network architecture.
2. Sign in online to your Routific backend console normally using administrative or owner-level developer permissions and acquire a unique authorization bearer token assigned selectively to you in Settings.
3. Paste the generated `Routific API Token` densely into the secure component form variables completely locked down below.
4. Issue organic text questions natively to the interface: "Generate a standalone route resolving 4 pending visits and subsequently publish it smoothly to the designated driver's Routific mobile app."

### Who is this for?

- **Fleet Owners & Dispatchers** — Dynamically alter and resolve ongoing jobs via simple conversational overrides without needing to fight with routing engine web variables when managing live chaos continuously natively.
- **Logistics Center Operations** — Fetch precise route matrices seamlessly containing granular ETAs dynamically parsed from the system without relying strictly upon legacy internal integrations proactively natively.
- **Enterprise Product Engineers** — Easily execute deep and massive asynchronous routing batches proactively through an intuitive text interface dynamically tied natively to standard APIs natively natively.


## Available Tools
- **cancel_saas_job**: This action is irreversible.

Cancels and deletes a delivery job from the platform
- **create_platform_route**: Creates a new route plan in the platform
- **create_saas_job**: Provide a JSON object with order details.

Creates a new delivery job in the platform
- **get_route_timeline**: Retrieves the stop-by-stop timeline for a route
- **list_platform_jobs**: Lists all delivery jobs in the Routific platform
- **poll_async_solution**: Polls the status of an asynchronous VRP job
- **publish_route_to_driver**: Publishes a route to the driver's mobile app
- **solve_async_vrp_long**: Returns a job ID for polling.

Submits a large Vehicle Routing Problem for asynchronous solving
- **solve_standalone_vrp**: Provide a JSON object with visits, fleet, and options.

Solves a standalone Vehicle Routing Problem synchronously
- **update_saas_job**: Updates an existing delivery job


## Installation & Usage

To install and use the **Routific** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/routific](https://vinkius.com/mcp/routific)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
