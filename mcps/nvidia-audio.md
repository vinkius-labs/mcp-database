# NVIDIA Audio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nvidia-audio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nvidia-audio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nvidia-audio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Transcribe speech, generate voices, translate audio, and clone voices via NVIDIA Audio APIs.

## Description
Connect **NVIDIA Audio** to any AI agent and unlock professional-grade audio processing — transcribe speech to text, generate natural voices, translate audio across languages, perform speaker diarization, and clone voices through natural conversation.

### What you can do
- **Speech-to-Text** — Transcribe audio files with high accuracy using Parakeel models
- **Text-to-Speech** — Convert text to natural-sounding speech
- **Audio Translation** — Translate spoken audio directly to another language
- **Speaker Diarization** — Identify and separate different speakers in audio
- **Voice Cloning** — Clone a voice from a sample and generate new speech
- **Noise Cancellation** — Remove background noise from recordings
- **Audio Classification** — Classify audio as speech, music, noise, etc.
- **Punctuation Restoration** — Add punctuation to raw speech-to-text output

### How it works
1. Subscribe to this server
2. Enter your NVIDIA API Key (from build.nvidia.com)
3. Start processing audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Transcription Services** — Automate meeting notes, podcast transcripts, and subtitles
- **Content Creators** — Generate voiceovers and clone voices for multilingual content
- **Customer Support** — Analyze call recordings with diarization and sentiment analysis


## Available Tools
- **list_audio_models**: List available audio models on NVIDIA API Catalog
- **classify_audio**: ) with confidence scores.

Classify the type of sound in an audio file
- **clone_voice**: Clone a voice from a reference audio and generate speech
- **cancel_noise**: Remove background noise from audio
- **speaker_diarization**: Identify different speakers in an audio file
- **punctuate_text**: Add punctuation and capitalization to raw text
- **speech_to_text**: Supports multiple languages. Provide a public audio URL (MP3, WAV, etc).

Transcribe speech from audio to text (Whisper-style)
- **summarize_audio**: Summarize an audio transcript
- **text_to_speech**: Optional voice parameter for different voices.

Convert text to natural-sounding speech
- **audio_translation**: Provide target language.

Translate spoken audio to another language


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NVIDIA Audio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe this meeting recording: https://example.com/meeting.mp3"

**🤖 AI Agent:**
> Transcription: 'Welcome everyone to the Q2 review. Our revenue grew 15% compared to last quarter...'

---

**👤 You:**
> "Convert this text to speech: 'Welcome to our presentation today.'"

**🤖 AI Agent:**
> Speech generated successfully! Audio data available for playback.

---

**👤 You:**
> "Identify different speakers in this call: https://example.com/call.wav"

**🤖 AI Agent:**
> Detected 3 speakers: Speaker 1 (0:00-2:30), Speaker 2 (2:31-5:45), Speaker 1 (5:46-8:20).


## Installation & Usage

To install and use the **NVIDIA Audio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nvidia-audio](https://vinkius.com/mcp/nvidia-audio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
