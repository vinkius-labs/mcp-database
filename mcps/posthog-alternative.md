# PostHog MCP Server

Manage product analytics and feature flags via PostHog — query events, inspect cohorts, toggle flags and create annotations from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/posthog-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

## Description
Connect your **PostHog** account to any AI agent and gain full control over your product analytics, feature flags and user cohorts through natural conversation.

### What you can do

- **User & Project Discovery** — Verify your account access and list all analytics projects
- **Feature Flag Management** — List, create, update and delete feature flags with rollout configuration
- **Cohort Inspection** — Review all behavioral cohorts and their filter definitions
- **Person Analytics** — Look up individual users by distinct ID, view their properties and activity timeline
- **Event Tracking** — Browse recent events, filter by event type and inspect event properties
- **Timeline Annotations** — Create and review annotations that correlate metric changes with deployments or launches

### How it works

1. Subscribe to this server
2. Enter your PostHog Personal API Key
3. Start managing your product analytics and feature flags from Claude, Cursor, or any MCP-compatible client

Stop switching between PostHog dashboards to check flag status or review event data. Your AI acts as a dedicated product analytics engineer.

### Who is this for?

- **Product Managers** — audit feature flag rollout percentages, review cohort definitions and create annotations for launches
- **Developers** — toggle feature flags, inspect event payloads and verify person properties without opening the PostHog UI
- **Data Analysts** — browse recent events, review person profiles and cohort membership for analysis


## Available Tools
- **create_annotation**: Annotations appear on insights graphs and help correlate metric changes with deployments, launches or incidents. Requires the content text. Optionally set a date_marker (ISO 8601 date).

Create a new annotation in PostHog
- **create_feature_flag**: Requires the flag key (unique identifier). Optionally set the name, description, enabled status, rollout percentage and filters. The key must be unique across all flags in the project.

Create a new PostHog feature flag
- **delete_feature_flag**: All targeting conditions, release conditions and experiment data associated with the flag will be deleted. Provide the numeric flag ID. WARNING: this action is irreversible.

Delete a PostHog feature flag
- **get_feature_flag**: Provide the numeric flag ID from list_feature_flags.

Get details for a specific PostHog feature flag
- **get_person**: Provide the distinct_id used to identify the person.

Get details for a specific person in PostHog
- **get_user**: Returns user ID, email, name, organization membership and permissions. Use this to verify your API key is working and check your access level.

Get the current PostHog user details
- **list_annotations**: Annotations are markers on timeline graphs that highlight important events like deployments, feature launches or incidents. Returns annotation ID, content, date marker and whether it is pinned.

List annotations in PostHog
- **list_cohorts**: Each cohort is a dynamic group of users defined by event-based or property-based filters. Returns cohort ID, name, description, whether it is calculated or static.

List behavioral cohorts in PostHog
- **list_events**: Optionally filter by event name (e.g. "pageview", "signup", "purchase") and set a limit. Each event includes the event name, timestamp, person distinct ID and properties.

List events tracked in PostHog
- **list_feature_flags**: Each flag has a key, name, enabled status, rollout percentage, filters and release conditions. Returns flag ID, key, name, whether it is active, and the targeting configuration. Use this to audit feature flag coverage.

List all feature flags in PostHog
- **list_persons**: Each person has distinct IDs, properties, creation date and last event timestamp. Optionally set limit (default 20) and offset for pagination.

List persons (users) tracked in PostHog
- **list_projects**: Each project is an analytics workspace with its own events, persons, feature flags and cohorts. Returns project ID, name, organization and creation date.

List PostHog projects
- **update_feature_flag**: Provide the flag ID and any fields to change: name, description, enabled status. Only the fields you provide will be updated.

Update an existing PostHog feature flag


## Installation & Usage

To install and use the **PostHog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/posthog-alternative](https://vinkius.com/mcp/posthog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
