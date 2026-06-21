# Render MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/render)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/render-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/render-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Equip your AI to orchestrate cloud infrastructure, manage service deployments, and execute scaling operations natively on your Render platform.

## Description
Connect your AI assistant directly to your **Render** cloud infrastructure via their official capabilities API. By granting your agent access to your hosting environments, you transform standard chat text into a powerful DevOps control center. Command deployments, scale back background workers to save costs, and instantiate brand-new services linked directly from your GitHub repositories without ever opening the Render dashboard.

### What you can do

- **Control Services & Spend** — Retrieve status checks on all active web endpoints, databases, and cron jobs (`list_services`). Instantly pause compute on unused projects using `suspend_service` and wake them back up later with `resume_service` to manage hosting costs.
- **Trigger & Monitor Deployments** — Inspect the deployment history for a specific application (`list_deploys`). Noticed a hotfix on GitHub? Tell your AI to forcefully restart the build pipeline executing `trigger_deploy` while optionally clearing the build cache.
- **Architect Environments** — Direct the agent to dynamically provision fresh infrastructure (`create_service`) pointing to a specific GitHub repository branch. Or easily swap which branch an existing project trails using `update_service_branch`.
- **Clean Up Infrastructure** — Quickly tear down obsolete staging instances permanently by instructing the AI via natural language to purge unwanted resources (`delete_service`).

### How it works

1. Install the Render platform extension module in your MCP.
2. Obtain your personal `Render API Key` from your Render Account Settings under the API Keys section. Insert it securely into the connection configuration below.
3. Chat with your AI using natural DevOps phrasing like: "List my web services, then suspend the one named 'old-staging-app'."

### Who is this for?

- **DevOps & Infrastructure Engineers** — Control routing, execute cache-cleared deployments, or suspend costly non-production workers directly from your command prompt logic.
- **Backend Developers** — Quickly spin up private services or background workers for new architectures by just typing a repo link in your chat window.
- **Startups & Indie Hackers** — Save time managing platform UI. Just ask your AI companion to identify, suspend, and analyze your app deployments natively in seconds.


## Available Tools
- **create_service**: Specify type, name, owner, and repository.

Creates a new Render service from a GitHub repository
- **delete_service**: This action is irreversible.

Permanently deletes a Render service
- **get_deploy**: Retrieves details for a specific deployment
- **get_service**: Retrieves details for a specific Render service
- **list_deploys**: Lists recent deployments for a service
- **list_services**: Lists all services (web apps, databases, cron jobs) in the Render account
- **resume_service**: Resumes a previously suspended service
- **suspend_service**: Suspends a service to stop execution and billing
- **trigger_deploy**: Triggers a manual deployment for a service
- **update_service_branch**: Updates the tracked GitHub branch for a service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Render** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my web services, then suspend the one named 'old-staging-app'."

**🤖 AI Agent:**
> I checked your services utilizing `list_services`. I found the matching instance ('old-staging-app', ID: srv-...a1s). By executing `suspend_service`, the application is now safely paused, terminating related compute billing operations momentarily until you need it again.

---

**👤 You:**
> "Check the recent deployment history for my main front-end service (srv-xyz123)."

**🤖 AI Agent:**
> Pulling data using the `list_deploys` interface on `srv-xyz123`, I can confirm the last 3 deployments occurred at [10:30 AM], [11:15 AM], and [1:00 PM]. The most recent deployment completed successfully and is live.

---

**👤 You:**
> "Trigger a force deployment on service ID 'srv-backend88' and clear its build cache."

**🤖 AI Agent:**
> Deploy triggered using `trigger_deploy` with instructions pointing at `srv-backend88`. As requested, I bypassed internal optimizations establishing a true clean slate by clearing the previous build cache prior to cloning code.


## Installation & Usage

To install and use the **Render** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/render](https://vinkius.com/mcp/render)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
