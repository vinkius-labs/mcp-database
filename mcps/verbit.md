# Verbit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/verbit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/verbit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/verbit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate professional transcription and captioning via Verbit — upload media, track job progress, and retrieve transcripts in multiple formats directly from your AI agent.

## Description
Connect your **Verbit** account to any AI agent to streamline your professional transcription and captioning workflows. This server allows you to handle high-quality speech-to-text tasks through simple conversation.

### What you can do

- **Transcription Jobs** — Create new transcription jobs by providing public media URLs and specifying languages.
- **Status Tracking** — Monitor the real-time progress and status of your transcription requests using unique job IDs.
- **Transcript Retrieval** — Download completed transcripts in various formats including JSON, TXT, SRT, VTT, or DOCX for immediate use.
- **External Referencing** — Tag jobs with external IDs to maintain consistency with your internal database or project management tools.

### How it works

1. Subscribe to this server
2. Enter your Verbit API Key
3. Start managing your transcription pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Media Teams** — quickly generate captions (SRT/VTT) for videos without leaving your workflow.
- **Legal & Academic Professionals** — automate the transcription of recordings and interviews into structured documents.
- **Product Managers** — integrate transcription status checks into automated project reports.


## Available Tools
- **create_job**: Upload a media file for transcription
- **get_job**: Check the progress of a transcription job
- **get_transcript**: Download the completed transcript


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Verbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a transcription job for this audio file: https://example.com/interview.mp3"

**🤖 AI Agent:**
> I've started the transcription job for your file. The Job ID is 'vbt_98765'. You can check its progress anytime.

---

**👤 You:**
> "What is the current status of Verbit job vbt_98765?"

**🤖 AI Agent:**
> Checking the status... Job 'vbt_98765' is currently at 75% progress and is in the 'In Progress' state.

---

**👤 You:**
> "Download the transcript for job vbt_98765 in Word format."

**🤖 AI Agent:**
> I've retrieved the transcript for job 'vbt_98765' in DOCX format. You can access the content here.


## Installation & Usage

To install and use the **Verbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/verbit](https://vinkius.com/mcp/verbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
