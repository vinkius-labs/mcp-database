# Sentry MCP Server

Grant your AI agent full access to Sentry's Application Performance Monitoring tools to track raw exceptions, resolve error logs, and inspect crash stack traces dynamically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sentry)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Sentry** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sentry](https://vinkius.com/mcp/sentry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
