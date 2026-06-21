# iCal Calendar Parser MCP Server

Parse exported .ics calendar files from Google Calendar, Apple Calendar, or Outlook local. Let your AI find free slots, count meetings, and manage your schedule.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ical-calendar-parser)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
Claude has no access to your local calendar. When you ask 'Do I have any free time tomorrow afternoon?', it simply cannot answer. But if you export your calendar as an `.ics` file (which every major calendar app supports), this MCP bridges the gap.

This engine uses a robust iCal parser to extract every event with its title, start/end times, location, and attendees into a clean JSON timeline. Sorted chronologically, the AI can instantly find conflicts, identify free slots, and generate weekly summaries of your schedule.

### The Superpowers

- **Universal Calendar Support:** Works with Google Calendar, Apple Calendar, Outlook, and any standard .ics file.
- **Chronological Sorting:** Events are automatically sorted by start date for timeline clarity.
- **Token-Safe:** Caps at 200 events to prevent context overflow.
- **100% Air-Gapped Privacy:** Your personal schedule stays on your machine.


## Available Tools
- **parse_ical_calendar**: ics). Provide the absolute file path.

Parse a local .ics calendar export (Google Calendar, Apple Calendar, Outlook) into structured JSON events offline


## Installation & Usage

To install and use the **iCal Calendar Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ical-calendar-parser](https://vinkius.com/mcp/ical-calendar-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
