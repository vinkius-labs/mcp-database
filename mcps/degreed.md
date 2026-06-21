# Degreed MCP Server

Equip your AI agent to discover learning content, track skills, and monitor user completions via the Degreed API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/degreed)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Degreed**, the leading upskilling and learning experience platform (LXP), directly into your AI workflow. Discover available learning content, monitor employee skill profiles, and track progress across pathways and plans using natural language.

### What you can do

- **Content Discovery** — Search the entire Degreed catalog for courses, articles, and videos matching specific keywords.
- **Skill Intelligence** — List and review the defined skills taxonomy and individual user skill profiles.
- **Learning Oversight** — Monitor user completions, active learning plans, and curated pathways.
- **User Research** — Retrieve detailed metadata and activity summaries for learners in your organization.

### How it works

1. Connect the Degreed integration to your AI assistant.
2. Authorize using your Degreed Client ID and Client Secret (found in your API settings).
3. Orchestrate your organization's learning and development through intuitive conversation.

### Who is this for?

- **L&D Managers** — Quickly check learner progress and content availability on the go.
- **Talent Partners** — Research employee skill sets and identify talent gaps via chat.
- **Team Leads** — Monitor team learning goals and pathway completions during planning.


## Available Tools
- **get_content_details**: Resolves detailed descriptions, associated skill tags, and duration metadata.

Get detailed metadata for a specific learning item
- **get_user_profile**: Resolves assigned skill ratings, learning progress, and active pathways within the Degreed ecosystem.

Get full profile and skill data for a specific user
- **list_active_learners**: Identifies users with recent completion activity within the Degreed workspace.

List users who have completed learning recently
- **list_learning_content**: Returns content metadata including titles, providers, content types (e.g., article, video, course), and external URLs.

List all available learning content in the Degreed catalog
- **list_learning_pathways**: Returns pathway metadata including objectives, total duration, and completion requirements.

List curated learning pathways available to users
- **list_learning_plans**: Returns active learning plans, including target completion dates and linked competencies.

List learning plans and goals configured in the system
- **list_defined_skills**: Returns the standardized list of skills and competencies defined by the organization for talent mapping.

List the skills taxonomy defined in your organization
- **list_user_completions**: Returns a history of all learned items with completion timestamps and earned skill points.

List all learning content completed by a specific user
- **list_degreed_users**: Returns a list of users with metadata including system IDs, professional titles, and organizational affiliations.

List all users registered in your Degreed organization
- **search_learning_catalog**: Matches terms against titles, descriptions, and skill tags to return a ranked list of relevant learning materials.

Search for learning content by keyword or term


## Installation & Usage

To install and use the **Degreed** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/degreed](https://vinkius.com/mcp/degreed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
