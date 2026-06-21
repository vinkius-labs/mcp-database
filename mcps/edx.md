# edX MCP Server

Search and discover online courses from Harvard, MIT, Berkeley and 160+ top institutions on edX.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/edx)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect to **edX** and explore the world's largest online learning platform through natural conversation — no API key needed.

### What you can do

- **Course Search** — Search thousands of courses by topic, university, level and language
- **Course Details** — Get full course info including descriptions, prerequisites and effort estimates
- **Course Runs** — Find upcoming and current course offerings with start dates and enrollment links
- **Programs** — Browse MicroMasters, Professional Certificates, XSeries and Bootcamps
- **Organizations** — Explore all partner universities and institutions (Harvard, MIT, Google, IBM)
- **Subjects** — Discover all subject categories available on the platform

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Discover online courses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Students** — find courses by topic, compare offerings from different universities and discover programs
- **Lifelong Learners** — explore subjects, discover MicroMasters and Professional Certificates
- **Educators** — research what courses are available, compare institutions and find learning paths


## Available Tools
- **get_course**: Returns title, description, organization, level, subjects, pacing, estimated effort, prerequisites and available course runs.

Get detailed info for a specific edX course
- **get_course_run**: Get details for a specific course run
- **get_course_runs**: Optionally filter by course key and status (upcoming, current, archived).

Get course runs (scheduled offerings) for courses
- **get_organizations**: Returns organization names, descriptions, logos and course counts. Includes Harvard, MIT, Berkeley, Google, IBM and many more.

Get partner organizations that offer courses on edX
- **get_program**: Get details for a specific edX program
- **get_subjects**: Returns subject names, descriptions and course counts. Useful for discovering what topics are covered on the platform.

Get course subject categories
- **search_courses**: Supports free-text search, filtering by organization, level (beginner/intermediate/advanced), language, subject. Returns course titles, descriptions, organizations, levels, subjects and enrollment links.

Search for online courses on edX
- **search_programs**: Includes MicroMasters, Professional Certificates, XSeries and Bootcamps. Returns program titles, descriptions, course counts and type.

Search for edX programs (MicroMasters, Professional Certificates, XSeries)


## Installation & Usage

To install and use the **edX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edx](https://vinkius.com/mcp/edx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
