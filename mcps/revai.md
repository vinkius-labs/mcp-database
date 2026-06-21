# Rev.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/revai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/revai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/revai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

High-accuracy speech-to-text and transcription — submit media files, generate AI summaries, and create captions directly from your AI agent.

## Description
Connect to **Rev AI** to transform your audio and video files into actionable text. This MCP server allows your AI agent to handle the entire transcription lifecycle—from submission to final summary.

### What you can do

- **Speech-to-Text** — Submit media URLs for asynchronous transcription using `submit_stt_job` with support for multiple languages and models (machine, human, fusion).
- **Job Management** — Track the status of your transcription jobs with `get_stt_job` and manage your history from the last 30 days using `list_stt_jobs`.
- **Transcripts & Captions** — Retrieve transcripts in JSON or text format with `get_transcript`, and generate SRT or VTT captions for video content using `get_captions`.
- **AI Summarization** — Automatically generate concise summaries of your completed transcripts using `get_transcript_summary` to save time.
- **Custom Vocabulary** — Improve accuracy for technical terms or unique names by submitting custom phrases via `submit_vocabulary`.

### How it works

1. Subscribe to this server
2. Enter your Rev AI Access Token
3. Start transcribing audio and video via Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Quickly generate captions and summaries for videos and podcasts to boost accessibility and SEO.
- **Researchers & Journalists** — Transcribe interviews and meetings to analyze qualitative data efficiently without manual typing.
- **Developers** — Integrate professional-grade STT capabilities into your AI workflows to process voice notes or meeting recordings.


## Available Tools
- **delete_stt_job**: Only allowed for completed or failed jobs.

Permanently delete job data
- **delete_vocabulary**: Delete a custom vocabulary
- **get_alignment_result**: Get aligned timestamps for a forced alignment job
- **get_captions**: Get captions for a completed job
- **get_language_id_result**: Get top language and confidence scores for a job
- **get_sentiment_analysis_result**: Get sentiment scores for a job
- **get_stt_job**: Get status and details of a transcription job
- **get_topic_extraction_result**: Get extracted topics and scores for a job
- **get_transcript_summary**: Get the summary for a completed transcript job
- **get_transcript**: Get the transcript for a completed job
- **get_vocabulary**: Check processing status of a custom vocabulary
- **list_stt_jobs**: Get a list of transcription jobs from the last 30 days
- **list_vocabularies**: List recent custom vocabularies
- **submit_alignment_job**: Submit audio and transcript for forced alignment
- **submit_language_id_job**: Submit an audio file/URL for language identification
- **submit_sentiment_analysis_job**: Submit a transcript for sentiment analysis
- **submit_stt_job**: Submit a media file for asynchronous transcription
- **submit_topic_extraction_job**: Submit a transcript for topic extraction
- **submit_vocabulary**: Submit a custom vocabulary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rev.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe this podcast episode: https://example.com/audio.mp3"

**🤖 AI Agent:**
> I've submitted the transcription job for your audio file. The Job ID is `abc-123`. I'll monitor the status for you.

---

**👤 You:**
> "Give me a summary of the transcript for job ID abc-123."

**🤖 AI Agent:**
> Here is the summary for job `abc-123`: The discussion focused on the new API deployment strategy and the timeline for the Q3 release.

---

**👤 You:**
> "List my transcription jobs from the last month."

**🤖 AI Agent:**
> I found 3 recent jobs: `abc-123` (transcribed), `def-456` (in_progress), and `ghi-789` (failed). Which one would you like to check?


## Installation & Usage

To install and use the **Rev.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revai](https://vinkius.com/mcp/revai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
