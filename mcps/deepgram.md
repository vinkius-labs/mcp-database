# Deepgram MCP Server

Power audio AI via Deepgram — perform high-speed speech-to-text, generate lifelike text-to-speech, track usage, and manage API keys directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deepgram)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Connect your **Deepgram** account to any AI agent and take full control of your speech-to-text (STT) and text-to-speech (TTS) workflows through natural conversation.

### What you can do

- **Speech-to-Text (STT)** — Dispatch automated transcription requests for remote audio URLs using the lightning-fast Nova-2 model to consume explicit WAV/MP3 web streams
- **Text-to-Speech (TTS)** — Generate high-fidelity audio from raw text using Aura voices, outputting the exact binary stream footprint natively from your chat
- **Usage Monitoring** — Analyze specific global bounds hitting `/usage` to map literally terabytes of exact API transcription times and TTS byte usage
- **Project & Key Management** — List and create ephemeral Deepgram access boundaries (API keys) and isolate organizational tenants where Audio AI billing is enforced
- **Wallet Oversight** — Retrieve explicit cloud logging tracing explicit Vault limits and verify direct wallet thresholds to ensure pipelines never drop
- **Identity & Invites** — Manage developer limits by listing members and sending team invites to specific project UUIDs strictly

### How it works

1. Subscribe to this server
2. Enter your Deepgram API Key (found in the Deepgram Console under Settings > API Keys)
3. Start managing your audio AI workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test STT/TTS models and manage API keys without leaving the development environment
- **Product Teams** — monitor audio AI usage and verify transcription accuracy in real-time
- **Data Engineers** — audit transcription volumes and manage project-wide audio pipelines using natural language
- **Ops Teams** — track wallet balances and manage team access across multiple Deepgram projects


## Available Tools
- **send_invite**: Invite a team member to a project
- **list_keys**: List API keys for a project
- **get_balances**: Get credit balances for a project
- **create_key**: Payload should include comment, scopes, and optional expiration.

Create a new API key for a project
- **delete_key**: Revoke and delete an API key
- **list_members**: List team members in a project
- **list_projects**: List all Deepgram projects in your account
- **transcribe_url**: Supports WAV, MP3, FLAC, and other formats.

Transcribe audio from a URL using Deepgram Nova-2
- **speak_text**: Returns metadata about the generated audio.

Convert text to speech using Deepgram Aura voices
- **get_usage**: Use query_string for date filters (e.g. "start=2026-01-01&end=2026-06-01").

Get API usage statistics for a project


## Installation & Usage

To install and use the **Deepgram** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepgram](https://vinkius.com/mcp/deepgram)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
