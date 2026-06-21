# Sentry MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sentry)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sentry-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sentry-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Grant your AI agent full access to Sentry's Application Performance Monitoring tools to track raw exceptions, resolve error logs, and inspect crash stack traces dynamically.

## Description
Equip your favorite LLM interface with direct, real-time investigative access over your application's **Sentry** operational environments. Skip the grueling task of combing through the rigid crash dashboard visually. Now, your AI can pull up the latest software exceptions directly into Cursor or an MCP-enabled chat window, read the contextual stack trace natively, and even close out resolved bugs.

### What you can do

- **Live Crash Monitoring** — Query the `list_issues` functionality at any time to instantly see which endpoints or functions are currently malfunctioning and throwing fatal alerts
- **Deep Error Inspection** — Feed an `issue_id` to the agent via `get_issue_details`. The LLM will devour the entire stack trace, evaluate the environmental metadata, and suggest precisely which lines of code need attention
- **Project & Organization Forensics** — Interrogate the AI regarding internal structures (`list_users`, `list_teams`) and easily scan separate software branches or repositories (`list_projects`) configured in your Sentry silo
- **Alert Triage (Mutable)** — Dictate the agent to close resolved items (`resolve_issue`), marking the exception safely as handled without having to load the web interface

### How it works

1. Simply activate this unified Server in your workflow configurations
2. Provide your overarching `Organization Slug` alongside your scoped `Auth Token` securely
3. Start pinging Claude asking: 'Why did my Vercel app crash 5 minutes ago on Sentry?'

### Who is this for?

- **Software Engineers** — fetch the specific `get_event_details` string natively in your IDE, feeding the LLM the exact variable state that shattered the production service
- **DevOps Engineers** — command the tool to `list_issues` occurring across European servers and quickly ascertain if a recent deploy caused a spike in latency
- **Technical Founders** — casually ask the chatbot for a summary of high-priority bugs open today across all startup projects before the daily standup


## Available Tools
- **delete_issue**: This action is irreversible.

Permanently deletes an issue
- **list_events**: Lists recent events for a project
- **get_event_details**: Retrieves details for a specific event
- **list_organizations**: Lists all Sentry organizations
- **list_projects**: Lists all projects in an organization
- **resolve_issue**: This is a reversible side-effect.

Resolves an issue in Sentry
- **list_organization_teams**: Lists all teams in an organization
- **list_organization_users**: Lists all users in an organization
- **get_issue_details**: Retrieves details for a specific issue
- **list_issues**: Lists all issues (errors) in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sentry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enumerate the most recently flared active open errors across the 'frontend-ui' project portal in Sentry."

**🤖 AI Agent:**
> I've successfully interrogated the Sentry API via `list_issues` scoping specifically down to the 'frontend-ui' project slug. Your dashboard flags 5 overarching unhandled exceptions aggressively repeating. The paramount threat ranks an ID marking 'TypeError: Cannot read properties of undefined (reading 'auth_token')' with ~4,200 events escalating in merely six hours. Should I invoke the agent to dig deep into this specific issue details block?

---

**👤 You:**
> "Fetch all pertinent internal parameters regarding issue id 6B3VX4921."

**🤖 AI Agent:**
> After meticulously scanning via `get_issue_details` parameter boundaries, issue block 6B3VX4921 centers around a PostgreSQL Deadlock collision error. The stack trace isolates its organic foundation originating from your `payment_processor.ts` dependency specifically on Line 132. Over 300 users were severely impacted since Tuesday. Noticeably, this fault correlates concurrently with a massive migration you pushed recently.

---

**👤 You:**
> "I've deployed a patch fixing the deadlock in db.ts. Mutate this specific issue globally to 'resolved'."

**🤖 AI Agent:**
> Got it. I've initiated an asynchronous payload signaling tool `resolve_issue` applied effectively corresponding to your specified ID within the active ecosystem. Subsequent polling shows this entity has correctly adopted the formal status value: 'RESOLVED'. Sentry charts will stop screaming out and notifying on channel hooks.


## Installation & Usage

To install and use the **Sentry** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sentry](https://vinkius.com/mcp/sentry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
