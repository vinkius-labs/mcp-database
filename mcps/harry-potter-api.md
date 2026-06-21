# Harry Potter API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harry-potter-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/harry-potter-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/harry-potter-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the wizarding world — search characters, students, staff, houses and spells from the Harry Potter universe.

## Description
Connect to the **Harry Potter API** and explore the wizarding world through natural conversation — no API key needed.

### What you can do

- **All Characters** — Browse the complete roster of Harry Potter characters and magical creatures
- **Hogwarts Students** — Find all students organized by house (Gryffindor, Slytherin, Ravenclaw, Hufflepuff)
- **Hogwarts Staff** — Discover teachers, professors and school staff
- **House Characters** — Filter characters by their Hogwarts house
- **Spells** — Explore the complete spellbook with names, types and effects

### How it works

1. Subscribe to this server
2. No API key needed — start exploring immediately
3. Discover Harry Potter data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free.

### Who is this for?

- **Harry Potter Fans** — discover character details, find which house characters belong to, and explore the spellbook
- **Trivia Enthusiasts** — explore patronuses, species, ancestry and alive status for every character
- **Writers & Creators** — get canonical character data for fan fiction, quizzes and content creation


## Available Tools
- **get_all_characters**: Each entry includes name, house, role (student/staff/creature), actor name, patronus, species and alive status. Useful for exploring the entire Harry Potter universe.

Get all Harry Potter characters and creatures
- **get_character**: Returns name, house, role, actor, patronus, species, ancestry and alive status. Use get_all_characters to find character IDs first.

Get a specific Harry Potter character by ID
- **get_house_characters**: Houses: gryffindor, slytherin, ravenclaw, hufflepuff. Each entry includes name, actor, role, patronus and species. Useful for exploring house-specific character rosters.

Get characters from a specific Hogwarts house
- **get_spells**: Each entry includes the spell name, type (charm, curse, hex, etc.) and effect description. Useful for discovering spells and their effects.

Get all Harry Potter spells
- **get_staff**: Each entry includes name, house, role, actor name and alive status. Useful for finding professors and school staff.

Get all Hogwarts staff and teachers
- **get_students**: Each entry includes name, house, year, actor name, patronus, species and alive status. Useful for finding students by house or character.

Get all Hogwarts students


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harry Potter API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all Gryffindor students."

**🤖 AI Agent:**
> Found 25+ Gryffindor students including: Harry Potter (stag patronus, half-blood), Hermione Granger (otter patronus, muggle-born), Ron Weasley (Jack Russell terrier patronus, pure-blood), Neville Longbottom, Ginny Weasley, Dean Thomas, Seamus Finnigan, Lavender Brown and more.

---

**👤 You:**
> "What spell creates a Patronus?"

**🤖 AI Agent:**
> The Expecto Patronum spell creates a Patronus. It's a charm that conjures a protective spirit guardian. The spell requires the caster to focus on a powerful happy memory. The Patronus takes the form of an animal unique to each wizard.

---

**👤 You:**
> "Who are all the Hogwarts staff members?"

**🤖 AI Agent:**
> Hogwarts staff includes: Albus Dumbledore (Headmaster, Gryffindor), Minerva McGonagall (Transfiguration, Gryffindor), Severus Snape (Potions/DADA, Slytherin), Filius Flitwick (Charms, Ravenclaw), Pomona Sprout (Herbology, Hufflepuff), Rubeus Hagrid (Care of Magical Creatures, Gryffindor), Argus Filch (caretaker), Sybill Trelawney (Divination) and more.


## Installation & Usage

To install and use the **Harry Potter API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harry-potter-api](https://vinkius.com/mcp/harry-potter-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
