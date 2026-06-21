# Yitu Technology / 依图科技 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yitu-technology)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yitu-technology-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yitu-technology-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

China's leading enterprise computer vision platform — perform facial recognition, search, and repository management via AI.

## Description
Empower your AI agent to orchestrate your enterprise-grade visual intelligence and facial recognition workflows with **Yitu Technology** (依图科技), a world-class provider of computer vision solutions. By connecting Yitu to your agent, you transform complex facial matching, identity search, and repository management into a natural conversation. Your agent can instantly detect faces in images, verify identities through high-precision comparison, manage custom facial repositories, and index new identities without you ever needing to navigate complex technical dashboards. Whether you are building an automated security checkpoint or managing a high-volume digital identity archive, your agent acts as a real-time computer vision coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Facial Orchestration** — Detect faces and extract precise locations and attributes from image URLs.
- **Identity Verification** — Perform high-precision 1:1 face comparison to verify if two images belong to the same person.
- **Library Search** — Search for matching identities within your private facial repositories (1:N recognition).
- **Repository Management** — Create, list, and monitor metadata for your facial data repositories.
- **Identity Indexing** — Register new faces and associate them with unique person identifiers for future search.

### How it works

1. Subscribe to this server
2. Enter your Yitu AppID (DevId) and APIKey (DevKey)
3. Start managing your visual identity infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise Security Teams** — automate access control monitoring and identity auditing through natural language queries.
- **App Developers** — integrate elite-level facial recognition capabilities into your AI-driven daily routines.
- **Operations Managers** — manage large-scale digital identity repositories directly from your AI-powered workspace.
- **Yitu Power Users** — integrate your existing facial recognition workflows into your AI-driven daily routines.


## Available Tools
- **detect_active_liveness**: Returns per-action pass/fail.

Active liveness detection with action verification
- **add_face_to_repo**: Register a face in a repository
- **compare_faces**: Verify if two faces match (1:1)
- **create_face_repo**: Create a new facial repository
- **delete_face_repo**: Delete a facial repository
- **detect_face**: Detect faces in an image
- **list_repos**: List all facial repositories
- **moderate_image**: Content moderation for images
- **ocr_id_card**: Extract text from an ID card image
- **remove_face_from_repo**: Remove a face from a repository
- **search_face_in_repo**: Returns top matches with confidence.

Search for a face in a repository (1:N)
- **detect_silent_liveness**: Detects photos, screens, and 3D masks.

Silent liveness detection (anti-spoofing)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yitu Technology / 依图科技** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Detect faces in this URL: [URL] and tell me how many people are there."

**🤖 AI Agent:**
> I've analyzed the image using Yitu Technology. I detected 3 unique faces in the photo. Would you like me to extract the facial locations or perform a comparison against your existing repositories?

---

**👤 You:**
> "Search for this face: [URL] in repository 'REPO_8821'."

**🤖 AI Agent:**
> I've performed a search in repository `REPO_8821`. I found a match with 98.2% confidence for Person ID `staff_042`. Should I retrieve the full metadata associated with this person?

---

**👤 You:**
> "List all facial repositories in my Yitu project."

**🤖 AI Agent:**
> I've retrieved the list of repositories. You have 2 active collections: 'HQ_Access_List' (ID: `rep_01`) and 'Visitor_Log' (ID: `rep_02`). Would you like me to check the statistics or add a new face to one of these?


## Installation & Usage

To install and use the **Yitu Technology / 依图科技** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yitu-technology](https://vinkius.com/mcp/yitu-technology)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
