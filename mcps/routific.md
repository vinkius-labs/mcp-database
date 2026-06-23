# Routific MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/routific)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI assistant to Routific to solve complex vehicle routing problems, dispatch drivers, and manage global delivery timelines natively through chat.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Routific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all current delivery jobs pending in the platform right now."

**🤖 AI Agent:**
> I requested the job details leveraging the `list_platform_jobs` command natively. Your portal correctly specifies 25 outstanding order elements natively. Let me know if you would like to begin inserting these naturally via `solve_async_vrp_long` to assemble your fleet dispatch timeline operations safely.

---

**👤 You:**
> "Generate a standalone route resolving 4 pending visits."

**🤖 AI Agent:**
> I've successfully generated a standalone route for the 4 pending visits using the `solve_standalone_vrp` solver. The total estimated driving time is 45 minutes, covering 12 miles. Would you like me to publish this route directly to the assigned driver?

---

**👤 You:**
> "Publish the finalized route to the designated driver's mobile app."

**🤖 AI Agent:**
> The finalized route has been successfully pushed to the designated driver's Routific mobile app. They should receive a notification and see the updated manifest shortly.


## ❓ FAQ

**Q: Can the AI push routes dynamically to drivers' smartphones automatically?**
Yes! Activating the `publish_route_to_driver` function dynamically interacts with the saas infrastructure, natively pushing an authorized manifest to the delivery team's active Routific phone apps flawlessly.

**Q: Does `solve_standalone_vrp` handle extremely large thousands of stops simultaneously efficiently?**
For very large batches, use `solve_async_vrp_long` instead. It processes the request asynchronously and you can poll for results with `poll_async_solution`. The standalone solver is best for smaller, real-time requests.

**Q: Can the integration update a delivery job after it has been created?**
Yes. Use `update_saas_job` to modify constraints, priorities, or delivery details on an existing job without having to delete and recreate it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/routific](https://vinkius.com/mcp/routific)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Routific** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `routific` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Routific** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "routific": {
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
